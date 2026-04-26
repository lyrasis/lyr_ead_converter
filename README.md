# lyr_ead_converter

ArchivesSpace plugin with updated version of the EAD converter

Current differences from stock ASpace:

  * Respects @label in `<unitdate>`
  * Removes trailing comma + whitespace from titles
  * Finding aid language and script default to English/Latin
  * Language of materials defaults to English/Latin
  * Publishes agents unless `audience="internal"`
  * Maps @id in `<dao>` and `<daogrp>` to map to `digital_object_id`. Note that in valid EAD, `<dao id="">` can't start with a number.
