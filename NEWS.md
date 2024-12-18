# NVIcheckmate 0.8.0 - (2024-12-13)

## New features:

- Created `assert_data_frame` with the argument `comment`.


# NVIcheckmate 0.7.3 - (2024-01-04)

## Bug fixes:

- Corrected error message in `match_arg` when `several.ok` = `FALSE` and lenght(x) > 1.


# NVIcheckmate 0.7.2 - (2023-12-14)

## Bug fixes:

- Removed warning in `match_arg` when `several.ok` = `FALSE` and lenght(x) > 1.


# NVIcheckmate 0.7.1 - (2023-12-13)
## Bug fixes:

- Now `match_arg` issues an error on all occasions when `several.ok` = `FALSE` and lenght(x) > 1.


## Other changes:

  - Updated README with improved installation instruction.
  
  
# NVIcheckmate 0.7.0 - (2023-11-19)

## New features:

  - Created `assert_integerish` with the argument `comment`.
  
  - `check_odbc_channel` and `assert_odbc_channel` now accept the argument dbinterface with the possible values c("odbc", "RODBC", "RPostgreSQL").


# NVIcheckmate 0.6.0 - (2023-01-23)

## New features:

  - `assert_disjunct` with the argument `comment` have been included.

  - `assert_integer` with the argument `comment` have been included.


## Other changes:

  - Included the NVIcheckmate reference manual in vignettes as pdf-file.
  
  - Updated README and corrected installation instruction.
  
  
# NVIcheckmate 0.5.0 - (2022-08-14)

## New features:

  - `assert_character` includes the arguments `n.char` and `max.char`.


## Other changes:

  - NVIcheckmate is adapted to and requires `checkmate` >= 2.1.0
  
  
# NVIcheckmate 0.4.0 - (2022-06-07)

## New features:

  - `match_arg` performs partial matching of arguments and includes the argument `ignore.case`. 


## Other changes:

  - Improved readability of error messages for `assert_choices_character` and `assert_subset_character`.
  
  - Updated README and vignette Contribute to NVIcheckmate.
  
  
# NVIcheckmate 0.3.3 - (2021-11-04)

## Bug fixes:

  - `assert_choices_character` and `assert_subset_character` now accepts argument `ignore.case` = "FALSE".
  
  
# NVIcheckmate 0.3.2 - (2021-09-28)

## Bug fixes:

  - `check_non_null` don't give a warning when input is a vector or data frame. Only check for `class` == NULL.
  
  
# NVIcheckmate 0.3.1 - (2021-09-27)

## Bug fixes:

  - Input to `check_non_missing` and `assert_non_missing` check corrected to list, not vector.
  
  
# NVIcheckmate 0.3.0 - (2021-09-16)

## New features:

  - `check_non_missing` and `assert_non_missing` check if at least one of two or more arguments are non_missing.
  
  
# NVIcheckmate 0.2.0 - (2021-09-05)

## New features:

  - `assert` now includes the argument `comment`.
  
  - `assert_character` with the argument `comment`.
  
  
## Other changes:

  - The order of arguments in assertion functions is changed so that `comment` is placed just before `add`.


# NVIcheckmate 0.1.0 - (2021-08-11)

## First release: 

Extension of checkmate with argument checking adapted for NVIverse

  - `check_package` and `assert_package` checks if a package is installed/attached.
  
  - `check_credentials` and `assert_credentials` checks if credentials (username and password) for specified services are saved in the users profile.
  
  - `check_odbc_channel` and `assert_odbc_channel` checks if an object is an open odbc channel.
  
  - `check_choices_character` is a wrapper around `checkmate::check_choices` with the argument: `ignore.case`.
  
  - `assert_choices_character` is a wrapper around `checkmate::assert_choices` with the arguments: `ignore.case` and `comment`.
  
  - `check_subset_character` is a wrapper around `checkmate::check_subset` with the argument: `ignore.case`.
  
  - `assert_subset_character` is a wrapper around `checkmate::assert_subset` with the arguments: `ignore.case` and `comment`.
  
  - `assert_names` is a modification of `checkmate::assert_names` with the argument: `comment`.
