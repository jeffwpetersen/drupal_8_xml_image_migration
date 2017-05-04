INTRODUCTION
------------
The drupal_8_xml_image_migration module is an example of a Drupal 8 migration of
an xml flat file with referenced images.

Requirements: content type 1 : children_book with 1 field: field_image

## BOOK AND IMAGE MIGRATION
------------
This module imports a list of books and corsponding images.

## XML FILE MIGRATION
------------
XML migration example.

## DRUPAL 8 IMAGE MIGRATION
------------
Migrate images and image fields

## Helpful drush migrate commands


drush mi --all,  migrate-import --all
drush migrate-import my_migration

enable the configraution manager module and use drush to update your configuratoion after changes.
drush config-import --partial --source=modules/drupal_8_xml_image_migration/config/install -y && drush migrate-import --group=book_data --update -y

MMSG migrate-messages will dispaly any error messages
drush mmsg program_image

MRS migrate-reset-status will halt any migrations that are stuck
drush mrs the_problem