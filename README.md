# lyr_ead_converter

ArchivesSpace plugin with updated version of the EAD converter

Current differences from stock ASpace:

* Respects @label in `<unitdate>`
* Removes trailing comma + whitespace from titles
* Finding aid language and script default to English/Latin
* Language of materials defaults to English/Latin
* Publishes agents unless `audience="internal"`
* Moves `<odd type="repository_processing_note">` to that field in resource and archival_object.
* Maps @id in `<dao>` and `<daogrp>` to `digital_object_id`. Note that in valid EAD, `<dao id="">` can't start with a number.
* Includes commented out block for handling `<dao>` and `<daogrp>` to link to existing digital objects via @id value.
* * WARNING: Use with caution!
* * `digital_object_id` must be unique in a repo, but not globally so be sure you are in the correct repo for upload.