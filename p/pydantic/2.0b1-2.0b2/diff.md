# Comparing `tmp/pydantic-2.0b1.tar.gz` & `tmp/pydantic-2.0b2.tar.gz`

## Comparing `pydantic-2.0b1.tar` & `pydantic-2.0b2.tar`

### file list

```diff
@@ -1,202 +1,202 @@
--rw-r--r--   0        0        0    79696 2020-02-02 00:00:00.000000 pydantic-2.0b1/HISTORY.md
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 pydantic-2.0b1/Makefile
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydantic-2.0b1/README.md
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/__init__.py
--rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_migration.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/alias_generators.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/class_validators.py
--rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/color.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/config.py
--rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/dataclasses.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/datetime_parse.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/decorator.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/env_settings.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/error_wrappers.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/errors.py
--rw-r--r--   0        0        0    37298 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/fields.py
--rw-r--r--   0        0        0     8882 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/functional_serializers.py
--rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/functional_validators.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/generics.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/json.py
--rw-r--r--   0        0        0    70647 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/json_schema.py
--rw-r--r--   0        0        0    54953 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/main.py
--rw-r--r--   0        0        0    38603 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/mypy.py
--rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/networks.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/py.typed
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/schema.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/tools.py
--rw-r--r--   0        0        0    15373 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/type_adapter.py
--rw-r--r--   0        0        0    37702 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/types.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/typing.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/utils.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/validate_call.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/validators.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_annotated_handlers.py
--rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    24182 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_decorators_v1.py
--rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0    66087 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    20566 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_known_annotated_metadata.py
--rw-r--r--   0        0        0    23972 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_schema_generation_shared.py
--rw-r--r--   0        0        0    37641 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    16535 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_validate_call.py
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/__init__.py
--rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/class_validators.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0    10595 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/decorator.py
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/tools.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/__init__.py
--rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/_hypothesis_plugin.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/annotated_types.py
--rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/class_validators.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/color.py
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/config.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/dataclasses.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/datetime_parse.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/decorator.py
--rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/env_settings.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/error_wrappers.py
--rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/errors.py
--rw-r--r--   0        0        0    50418 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/fields.py
--rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/generics.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/json.py
--rw-r--r--   0        0        0    44378 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/main.py
--rw-r--r--   0        0        0    38097 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/mypy.py
--rw-r--r--   0        0        0    21826 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/networks.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/py.typed
--rw-r--r--   0        0        0    47615 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/schema.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/tools.py
--rw-r--r--   0        0        0    35219 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/types.py
--rw-r--r--   0        0        0    19358 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/typing.py
--rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/utils.py
--rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/validators.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/__init__.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/conftest.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_abc.py
--rw-r--r--   0        0        0    14786 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_aliases.py
--rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_annotated.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_assert_in_validators.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_callable.py
--rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_color.py
--rw-r--r--   0        0        0    16774 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_computed_fields.py
--rw-r--r--   0        0        0    21049 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_config.py
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_construction.py
--rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_create_model.py
--rw-r--r--   0        0        0    63335 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_dataclasses.py
--rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_datetime.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_decorators.py
--rw-r--r--   0        0        0    20440 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_deprecated.py
--rw-r--r--   0        0        0    12182 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_deprecated_validate_arguments.py
--rw-r--r--   0        0        0    40531 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_discriminated_union.py
--rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_docs.py
--rw-r--r--   0        0        0    76384 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_edge_cases.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_errors.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_exports.py
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_fastapi.sh
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_fastapi_json_schema.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_fields.py
--rw-r--r--   0        0        0    26896 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_forward_ref.py
--rw-r--r--   0        0        0    71065 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_generics.py
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_internal.py
--rw-r--r--   0        0        0    13165 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_json.py
--rw-r--r--   0        0        0   140193 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_json_schema.py
--rw-r--r--   0        0        0    65906 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_main.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_migration.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_model_signature.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_model_validator.py
--rw-r--r--   0        0        0    29249 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_networks.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_networks_ipaddress.py
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_parse.py
--rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_prepare_annotations.py
--rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_private_attributes.py
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_pydantic_settings.sh
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_rich_repr.py
--rw-r--r--   0        0        0    10304 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_root_model.py
--rw-r--r--   0        0        0    29452 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_serialize.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_strict.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_structural_pattern_matching.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_tools.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_type_adapter.py
--rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_type_alias_type.py
--rw-r--r--   0        0        0   177998 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_types.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_types_namedtuple.py
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_types_payment_card_number.py
--rw-r--r--   0        0        0    25240 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_types_typeddict.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_typing.py
--rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_v1.py
--rw-r--r--   0        0        0    19485 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_validate_call.py
--rw-r--r--   0        0        0    72494 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_validators.py
--rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_validators_dataclass.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/__init__.py
--rw-r--r--   0        0        0    10878 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/test_mypy.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/mypy-plugin-strict-no-any.ini
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/mypy-plugin-strict.ini
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/mypy-plugin.ini
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/pyproject-default.toml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/pyproject-plugin-bad-param.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/pyproject-plugin-strict.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/pyproject-plugin.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/computed_fields.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/custom_constructor.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/dataclass_no_any.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail1.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail2.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail3.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail4.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail_defaults.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_default_factory.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_fail.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_success.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/success.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/computed_fields.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/custom_constructor.txt
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail1.txt
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail2.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail3.txt
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail4.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail_defaults.txt
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-strict.txt
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-success-strict.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin_default_factory.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin_success.txt
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/v1.0.1/fail1.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/v1.0.1/fail2.txt
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/v1.0.1/plugin_success.txt
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/pyright/pyproject.toml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/pyright/pyright_example.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pydantic-2.0b1/.gitignore
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.0b1/LICENSE
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 pydantic-2.0b1/pyproject.toml
--rw-r--r--   0        0        0   114997 2020-02-02 00:00:00.000000 pydantic-2.0b1/PKG-INFO
+-rw-r--r--   0        0        0    79910 2020-02-02 00:00:00.000000 pydantic-2.0b2/HISTORY.md
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 pydantic-2.0b2/Makefile
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydantic-2.0b2/README.md
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/__init__.py
+-rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_migration.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/alias_generators.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/color.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/config.py
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/dataclasses.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/datetime_parse.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/decorator.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/env_settings.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/errors.py
+-rw-r--r--   0        0        0    37298 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/fields.py
+-rw-r--r--   0        0        0     8882 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/functional_serializers.py
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/functional_validators.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/generics.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/json.py
+-rw-r--r--   0        0        0    70692 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/json_schema.py
+-rw-r--r--   0        0        0    54924 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/main.py
+-rw-r--r--   0        0        0    38603 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/mypy.py
+-rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/networks.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/py.typed
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/schema.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/tools.py
+-rw-r--r--   0        0        0    15617 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/type_adapter.py
+-rw-r--r--   0        0        0    37702 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/types.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/typing.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/utils.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/validate_call.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/validators.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_annotated_handlers.py
+-rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    24182 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    65337 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_known_annotated_metadata.py
+-rw-r--r--   0        0        0    23972 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_schema_generation_shared.py
+-rw-r--r--   0        0        0    37641 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    16535 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/class_validators.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10595 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/__init__.py
+-rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/annotated_types.py
+-rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/class_validators.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/color.py
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/config.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/dataclasses.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/datetime_parse.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/decorator.py
+-rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/env_settings.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/error_wrappers.py
+-rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/errors.py
+-rw-r--r--   0        0        0    50418 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/fields.py
+-rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/generics.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/json.py
+-rw-r--r--   0        0        0    44378 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/main.py
+-rw-r--r--   0        0        0    38097 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/mypy.py
+-rw-r--r--   0        0        0    21826 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/networks.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/py.typed
+-rw-r--r--   0        0        0    47615 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/schema.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/tools.py
+-rw-r--r--   0        0        0    35219 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/types.py
+-rw-r--r--   0        0        0    19358 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/typing.py
+-rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/utils.py
+-rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/validators.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydantic-2.0b2/pydantic/v1/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/__init__.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/conftest.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_abc.py
+-rw-r--r--   0        0        0    14786 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_aliases.py
+-rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_annotated.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_assert_in_validators.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_callable.py
+-rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_color.py
+-rw-r--r--   0        0        0    16774 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_computed_fields.py
+-rw-r--r--   0        0        0    21049 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_config.py
+-rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_construction.py
+-rw-r--r--   0        0        0    15857 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_create_model.py
+-rw-r--r--   0        0        0    63792 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_dataclasses.py
+-rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_datetime.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_decorators.py
+-rw-r--r--   0        0        0    20818 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_deprecated.py
+-rw-r--r--   0        0        0    12182 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_deprecated_validate_arguments.py
+-rw-r--r--   0        0        0    40531 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_discriminated_union.py
+-rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_docs.py
+-rw-r--r--   0        0        0    76384 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_edge_cases.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_errors.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_exports.py
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_fastapi.sh
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_fastapi_json_schema.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_fields.py
+-rw-r--r--   0        0        0    26896 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_forward_ref.py
+-rw-r--r--   0        0        0    71997 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_generics.py
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_internal.py
+-rw-r--r--   0        0        0    13165 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_json.py
+-rw-r--r--   0        0        0   140193 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_json_schema.py
+-rw-r--r--   0        0        0    68360 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_main.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_migration.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_model_signature.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_model_validator.py
+-rw-r--r--   0        0        0    29249 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_networks.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_networks_ipaddress.py
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_parse.py
+-rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_prepare_annotations.py
+-rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_private_attributes.py
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_pydantic_settings.sh
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_rich_repr.py
+-rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_root_model.py
+-rw-r--r--   0        0        0    29452 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_serialize.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_strict.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_structural_pattern_matching.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_tools.py
+-rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_type_adapter.py
+-rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_type_alias_type.py
+-rw-r--r--   0        0        0   178255 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_types.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_types_namedtuple.py
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_types_payment_card_number.py
+-rw-r--r--   0        0        0    25240 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_types_typeddict.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_typing.py
+-rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_v1.py
+-rw-r--r--   0        0        0    19653 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_validate_call.py
+-rw-r--r--   0        0        0    72997 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_validators.py
+-rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_validators_dataclass.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/__init__.py
+-rw-r--r--   0        0        0    10878 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/test_mypy.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/mypy-plugin-strict-no-any.ini
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/mypy-plugin-strict.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/mypy-plugin.ini
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/pyproject-default.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/pyproject-plugin-bad-param.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/pyproject-plugin-strict.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/configs/pyproject-plugin.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/computed_fields.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/custom_constructor.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/dataclass_no_any.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail1.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail2.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail3.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail4.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/fail_defaults.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_default_factory.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_fail.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_success.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/modules/success.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/computed_fields.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/custom_constructor.txt
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail1.txt
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail2.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail3.txt
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail4.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/fail_defaults.txt
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-strict.txt
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin-success-strict.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin_default_factory.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin_success.txt
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/v1.0.1/fail1.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/v1.0.1/fail2.txt
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/v1.0.1/plugin_success.txt
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/pyright/pyproject.toml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.0b2/tests/pyright/pyright_example.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pydantic-2.0b2/.gitignore
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.0b2/LICENSE
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 pydantic-2.0b2/pyproject.toml
+-rw-r--r--   0        0        0   115211 2020-02-02 00:00:00.000000 pydantic-2.0b2/PKG-INFO
```

### Comparing `pydantic-2.0b1/HISTORY.md` & `pydantic-2.0b2/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v2.0b2 (2023-06-03)
+
+Add `from_attributes` runtime flag to `TypeAdapter.validate_python` and `BaseModel.model_validate`.
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b2)
+
 ## v2.0b1 (2023-06-01)
 
 First beta pre-release of Pydantic V2
 
 See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b1)
 
 ## v2.0a4 (2023-05-05)
```

### Comparing `pydantic-2.0b1/Makefile` & `pydantic-2.0b2/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/README.md` & `pydantic-2.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/__init__.py` & `pydantic-2.0b2/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_migration.py` & `pydantic-2.0b2/pydantic/_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/alias_generators.py` & `pydantic-2.0b2/pydantic/alias_generators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/color.py` & `pydantic-2.0b2/pydantic/color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/config.py` & `pydantic-2.0b2/pydantic/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/dataclasses.py` & `pydantic-2.0b2/pydantic/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/errors.py` & `pydantic-2.0b2/pydantic/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 # We use this URL to allow for future flexibility about how we host the docs, while allowing for Pydantic
 # code in the while with "old" URLs to still work.
 # 'u' refers to "user errors" - e.g. errors caused by developers using pydantic, as opposed to validation errors.
 DEV_ERROR_DOCS_URL = f'https://errors.pydantic.dev/{VERSION}/u/'
 PydanticErrorCodes = Literal[
     'class-not-fully-defined',
+    'custom-json-schema',
     'decorator-missing-field',
     'discriminator-no-field',
     'discriminator-alias-type',
     'discriminator-needs-literal',
     'discriminator-alias',
     'typed-dict-version',
     'model-field-overridden',
```

### Comparing `pydantic-2.0b1/pydantic/fields.py` & `pydantic-2.0b2/pydantic/fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/functional_serializers.py` & `pydantic-2.0b2/pydantic/functional_serializers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/functional_validators.py` & `pydantic-2.0b2/pydantic/functional_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/json_schema.py` & `pydantic-2.0b2/pydantic/json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,16 +821,14 @@
     def _extract_discriminator(
         self, schema: core_schema.TaggedUnionSchema, one_of_choices: list[_JsonDict]
     ) -> str | None:
         """
         Extract a compatible OpenAPI discriminator from the schema and one_of choices that end up in the final schema.
         """
         openapi_discriminator: str | None = None
-        if 'discriminator' not in schema:
-            return None
 
         if isinstance(schema['discriminator'], str):
             return schema['discriminator']
 
         if isinstance(schema['discriminator'], list):
             # If the discriminator is a single item list containing a string, that is equivalent to the string case
             if len(schema['discriminator']) == 1 and isinstance(schema['discriminator'][0], str):
@@ -859,14 +857,15 @@
                 if alias_is_present_on_all_choices:
                     openapi_discriminator = alias
                     break
         return openapi_discriminator
 
     def chain_schema(self, schema: core_schema.ChainSchema) -> JsonSchemaValue:
         # Note: If we wanted to generate a schema for the _serialization_, would want to use the _last_ step:
+        # There are always more than zero steps, since the ChainSchema is validated on the pydantic-core side.
         return self.generate_inner(schema['steps'][0])
 
     def lax_or_strict_schema(self, schema: core_schema.LaxOrStrictSchema) -> JsonSchemaValue:
         """
         LaxOrStrict will use the strict branch for serialization internally,
         unless it was overridden here.
         """
```

### Comparing `pydantic-2.0b1/pydantic/main.py` & `pydantic-2.0b2/pydantic/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,27 +66,30 @@
 
     * `model_fields` is a class attribute that contains the fields defined on the model in Pydantic V2.
         This replaces `Model.__fields__` from Pydantic V1.
     *  `__pydantic_decorators__` contains the decorators defined on the model in Pydantic V2. This replaces
         `Model.__validators__` and `Model.__root_validators__` from Pydantic V1.
 
     Attributes:
-        __pydantic_validator__ (typing.ClassVar[SchemaValidator]): Validator for checking schema validity.
-        __pydantic_core_schema__ (typing.ClassVar[CoreSchema]): Schema for representing the model's core.
-        __pydantic_serializer__ (typing.ClassVar[SchemaSerializer]): Serializer for the schema.
-        __pydantic_decorators__ (_decorators.DecoratorInfos): Metadata for `@field_validator`, `@root_validator`,
+        __pydantic_validator__: Validator for checking schema validity.
+        __pydantic_core_schema__: Schema for representing the model's core.
+        __pydantic_serializer__: Serializer for the schema.
+        __pydantic_decorators__: Metadata for `@field_validator`, `@root_validator`,
             and `@serializer` decorators.
-        model_fields (typing.ClassVar[dict[str, FieldInfo]]): Fields in the model.
-        __signature__ (typing.ClassVar[Signature]): Signature for instantiating the model.
-        __private_attributes__ (typing.ClassVar[dict[str, ModelPrivateAttr]]): Private attributes of the model.
-        __class_vars__ (typing.ClassVar[set[str]]): Class variables of the model.
-        __pydantic_fields_set__ (set[str]): Set of fields in the model.
-        __pydantic_extra__ (typing.Optional[dict[str, Any]]): Extra fields in the model.
-        __pydantic_generic_metadata__ (_generics.PydanticGenericMetadata): Metadata for generic models.
-        __pydantic_parent_namespace__ (typing.Optional[dict[str, Any]]): Parent namespace of the model.
+        model_fields: Fields in the model.
+        __signature__: Signature for instantiating the model.
+        __private_attributes__: Private attributes of the model.
+        __class_vars__: Class variables of the model.
+        __pydantic_fields_set__: Set of fields in the model.
+        __pydantic_extra__: Extra fields in the model.
+        __pydantic_private__: Private fields in the model.
+        __pydantic_generic_metadata__: Metadata for generic models.
+        __pydantic_parent_namespace__: Parent namespace of the model.
+        __pydantic_custom_init__: Custom init of the model.
+        __pydantic_post_init__: Post init of the model.
     """
 
     if typing.TYPE_CHECKING:
         # populated by the metaclass, defined here to help IDEs only
         __pydantic_validator__: typing.ClassVar[SchemaValidator]
         __pydantic_core_schema__: typing.ClassVar[CoreSchema]
         __pydantic_serializer__: typing.ClassVar[SchemaSerializer]
@@ -139,21 +142,21 @@
     @classmethod
     def __get_pydantic_core_schema__(
         cls, __source: type[BaseModel], __handler: _annotated_handlers.GetCoreSchemaHandler
     ) -> CoreSchema:
         """Hook into generating the model's CoreSchema.
 
         Args:
-            __source (type[BaseModel]): The class we are generating a schema for.
+            __source: The class we are generating a schema for.
                 This will generally be the same as the `cls` argument if this is a classmethod.
-            __handler (GetJsonSchemaHandler): Call into Pydantic's internal JSON schema generation.
+            __handler: Call into Pydantic's internal JSON schema generation.
                 A callable that calls into Pydantic's internal CoreSchema generation logic.
 
         Returns:
-            CoreSchema: A `pydantic-core` `CoreSchema`.
+            A `pydantic-core` `CoreSchema`.
         """
         # Only use the cached value from this _exact_ class; we don't want one from a parent class
         # This is why we check `cls.__dict__` and don't use `cls.__pydantic_core_schema__` or similar.
         if '__pydantic_core_schema__' in cls.__dict__:
             # Due to the way generic classes are built, it's possible that an invalid schema may be temporarily
             # set on generic classes. I think we could resolve this to ensure that we get proper schema caching
             # for generics, but for simplicity for now, we just always rebuild if the class has a generic origin.
@@ -167,46 +170,48 @@
         cls,
         __core_schema: CoreSchema,
         __handler: _annotated_handlers.GetJsonSchemaHandler,
     ) -> JsonSchemaValue:
         """Hook into generating the model's JSON schema.
 
         Args:
-            __core_schema (CoreSchema): A `pydantic-core` CoreSchema.
+            __core_schema: A `pydantic-core` CoreSchema.
                 You can ignore this argument and call the handler with a new CoreSchema,
                 wrap this CoreSchema (`{'type': 'nullable', 'schema': current_schema}`),
                 or just call the handler with the original schema.
-            __handler (GetJsonSchemaHandler): Call into Pydantic's internal JSON schema generation.
+            __handler: Call into Pydantic's internal JSON schema generation.
                 This will raise a `pydantic.errors.PydanticInvalidForJsonSchema` if JSON schema
                 generation fails.
                 Since this gets called by `BaseModel.model_json_schema` you can override the
                 `schema_generator` argument to that function to change JSON schema generation globally
                 for a type.
 
         Returns:
-            JsonSchemaValue: A JSON schema, as a Python object.
+            A JSON schema, as a Python object.
         """
         return __handler(__core_schema)
 
     if typing.TYPE_CHECKING:
 
         def __init_subclass__(cls, **kwargs: Unpack[ConfigDict]):
             """
             This signature is included purely to help type-checkers check arguments to class declaration, which
             provides a way to conveniently set model_config key/value pairs:
 
-                class MyModel(BaseModel, extra='allow'):
-                    ...
+            ```py
+            class MyModel(BaseModel, extra='allow'):
+                ...
+            ```
 
             However, this may be deceiving, since the _actual_ calls to `__init_subclass__` will not receive any
             of the config arguments, and will only receive any keyword arguments passed during class initialization
             that are _not_ expected keys in ConfigDict. (This is due to the way `ModelMetaclass.__new__` works.)
 
             Args:
-                **kwargs (Unpack[ConfigDict]): Keyword arguments passed to the class definition, which set model_config
+                **kwargs: Keyword arguments passed to the class definition, which set model_config
             """
 
     @classmethod
     def __pydantic_init_subclass__(cls, **kwargs: Any) -> None:
         """
         This is intended to behave just like `__init_subclass__`, but is called by `ModelMetaclass`
         only after the class is actually fully initialized. In particular, attributes like `model_fields` will
@@ -216,40 +221,48 @@
         and it would require a prohibitively large refactor to the `ModelMetaclass` to ensure that
         `type.__new__` was called in such a manner that the class would already be sufficiently initialized.
 
         This will receive the same `kwargs` that would be passed to the standard `__init_subclass__`, namely,
         any kwargs passed to the class definition that aren't used internally by pydantic.
 
         Args:
-            **kwargs (Any): Any keyword arguments passed to the class definition that aren't used internally
+            **kwargs: Any keyword arguments passed to the class definition that aren't used internally
             by pydantic.
         """
         pass
 
     @classmethod
     def model_validate(
-        cls: type[Model], obj: Any, *, strict: bool | None = None, context: dict[str, Any] | None = None
+        cls: type[Model],
+        obj: Any,
+        *,
+        strict: bool | None = None,
+        from_attributes: bool | None = None,
+        context: dict[str, Any] | None = None,
     ) -> Model:
         """Validate a pydantic model instance.
 
         Args:
-            cls (type[Model]): The model class to use.
-            obj (Any): The object to validate.
-            strict (bool | None, optional): Whether to raise an exception on invalid fields. Defaults to None.
-            context (dict[str, Any] | None, optional): Additional context to pass to the validator. Defaults to None.
+            cls: The model class to use.
+            obj: The object to validate.
+            strict: Whether to raise an exception on invalid fields. Defaults to None.
+            from_attributes: Whether to extract data from object attributes. Defaults to None.
+            context: Additional context to pass to the validator. Defaults to None.
 
         Raises:
             ValidationError: If the object could not be validated.
 
         Returns:
-            Model: The validated model instance.
+            The validated model instance.
         """
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
-        return cls.__pydantic_validator__.validate_python(obj, strict=strict, context=context)
+        return cls.__pydantic_validator__.validate_python(
+            obj, strict=strict, from_attributes=from_attributes, context=context
+        )
 
     @property
     def model_fields_set(self) -> set[str]:
         """
         Returns the set of fields that have been set on this model instance.
 
         Returns:
@@ -270,38 +283,36 @@
 
     @property
     def model_computed_fields(self) -> dict[str, ComputedFieldInfo]:
         """
         Get the computed fields of this model instance.
 
         Returns:
-            Dict: A dictionary of computed field names and their corresponding `ComputedFieldInfo` objects.
+            A dictionary of computed field names and their corresponding `ComputedFieldInfo` objects.
         """
         return {k: v.info for k, v in self.__pydantic_decorators__.computed_fields.items()}
 
     @classmethod
     def model_validate_json(
         cls: type[Model],
         json_data: str | bytes | bytearray,
         *,
         strict: bool | None = None,
         context: dict[str, Any] | None = None,
     ) -> Model:
-        """Validate the given JSON data against the Pydantic model.
+        """
+        Validate the given JSON data against the Pydantic model.
 
         Args:
-            cls (type[Model]): The Pydantic model class to validate against.
-            json_data (Union[str, bytes, bytearray]): The JSON data to validate.
-
-        Keyword Args:
-            strict (Optional[bool]): Whether to enforce types strictly (default: `None`).
-            context (Optional[Dict[str, Any]]): Extra variables to pass to the validator (default: `None`).
+            json_data: The JSON data to validate.
+            strict: Whether to enforce types strictly (default: `None`).
+            context: Extra variables to pass to the validator (default: `None`).
 
         Returns:
-            Model: The validated Pydantic model.
+            The validated Pydantic model.
 
         Raises:
             ValueError: If `json_data` is not a JSON string.
         """
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
         return cls.__pydantic_validator__.validate_json(json_data, strict=strict, context=context)
@@ -379,29 +390,28 @@
         round_trip: bool = False,
         warnings: bool = True,
     ) -> dict[str, Any]:
         """
         Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
 
         Args:
-            self (object): The instance of the class that this method is attached to.
-            mode (Literal['json', 'python'] | str): The mode in which `to_python` should run.
+            mode: The mode in which `to_python` should run.
                 If mode is 'json', the dictionary will only contain JSON serializable types.
                 If mode is 'python', the dictionary may contain any Python objects.
-            include (Optional[List[str]]): A list of fields to include in the output.
-            exclude (Optional[List[str]]): A list of fields to exclude from the output.
-            by_alias (bool): Whether to use the field's alias in the dictionary key if defined.
-            exclude_unset (bool): Whether to exclude fields that are unset or None from the output.
-            exclude_defaults (bool): Whether to exclude fields that are set to their default value from the output.
-            exclude_none (bool): Whether to exclude fields that have a value of None from the output.
-            round_trip (bool): Whether to enable serialization and deserialization round-trip support.
-            warnings (bool): Whether to log warnings when invalid fields are encountered.
+            include: A list of fields to include in the output.
+            exclude: A list of fields to exclude from the output.
+            by_alias: Whether to use the field's alias in the dictionary key if defined.
+            exclude_unset: Whether to exclude fields that are unset or None from the output.
+            exclude_defaults: Whether to exclude fields that are set to their default value from the output.
+            exclude_none: Whether to exclude fields that have a value of None from the output.
+            round_trip: Whether to enable serialization and deserialization round-trip support.
+            warnings: Whether to log warnings when invalid fields are encountered.
 
         Returns:
-            Dict: A dictionary representation of the model.
+            A dictionary representation of the model.
         """
         return self.__pydantic_serializer__.to_python(
             self,
             mode=mode,
             by_alias=by_alias,
             include=include,
             exclude=exclude,
@@ -425,30 +435,26 @@
         round_trip: bool = False,
         warnings: bool = True,
     ) -> str:
         """
         Generates a JSON representation of the model using Pydantic's `to_json` method.
 
         Args:
-            indent (Optional[int]): Indentation to use in the JSON output. If None is passed, the output will be
-                compact.
-            include (Optional[Union[str, Set[str]]]): Field(s) to include in the JSON output. Can take either a string
-                or set of strings.
-            exclude (Optional[Union[str, Set[str]]]): Field(s) to exclude from the JSON output. Can take either a
-                string or set of strings.
-            by_alias (bool): Whether to serialize using field aliases. Defaults to False.
-            exclude_unset (bool): Whether to exclude fields that have not been explicitly set. Defaults to False.
-            exclude_defaults (bool): Whether to exclude fields that have the default value. Defaults to False.
-            exclude_none (bool): Whether to exclude fields that have a value of None. Defaults to False.
-            round_trip (bool): Whether to use serialization/deserialization between JSON and class instance. Defaults
-                to False.
-            warnings (bool): Whether to show any warnings that occurred during serialization. Defaults to True.
+            indent: Indentation to use in the JSON output. If None is passed, the output will be compact.
+            include: Field(s) to include in the JSON output. Can take either a string or set of strings.
+            exclude: Field(s) to exclude from the JSON output. Can take either a string or set of strings.
+            by_alias: Whether to serialize using field aliases. Defaults to False.
+            exclude_unset: Whether to exclude fields that have not been explicitly set. Defaults to False.
+            exclude_defaults: Whether to exclude fields that have the default value. Defaults to False.
+            exclude_none: Whether to exclude fields that have a value of None. Defaults to False.
+            round_trip: Whether to use serialization/deserialization between JSON and class instance. Defaults to False.
+            warnings: Whether to show any warnings that occurred during serialization. Defaults to True.
 
         Returns:
-            str: A JSON string representation of the model.
+            A JSON string representation of the model.
         """
         return self.__pydantic_serializer__.to_json(
             self,
             indent=indent,
             include=include,
             exclude=exclude,
             by_alias=by_alias,
@@ -465,20 +471,20 @@
         Creates a new instance of the `Model` class with validated data.
 
         Creates a new model setting `__dict__` and `__pydantic_fields_set__` from trusted or pre-validated data.
         Default values are respected, but no other validation is performed.
         Behaves as if `Config.extra = 'allow'` was set since it adds all passed values
 
         Args:
-            cls (type[Model]): The `Model` class.
-            _fields_set (set[str], optional): The set of field names accepted for the Model instance.
-            values (Any): Trusted or pre-validated data dictionary.
+            cls: The `Model` class.
+            _fields_set: The set of field names accepted for the Model instance.
+            values: Trusted or pre-validated data dictionary.
 
         Returns:
-            Model: A new instance of the `Model` class with validated data.
+            A new instance of the `Model` class with validated data.
         """
         m = cls.__new__(cls)
         fields_values: dict[str, Any] = {}
         for name, field in cls.model_fields.items():
             if field.alias and field.alias in values:
                 fields_values[name] = values[field.alias]
             elif name in values:
@@ -519,21 +525,20 @@
         Generates a JSON schema for a model class.
 
         To override the logic used to generate the JSON schema, you can create a subclass of `GenerateJsonSchema`
         with your desired modifications, then override this method on a custom base class and set the default
         value of `schema_generator` to be your subclass.
 
         Args:
-            cls (type): The model class for which the JSON schema is to be generated.
-            by_alias (bool): Whether to use attribute aliases or not. Defaults to `True`.
-            ref_template (str): The reference template. Defaults to `DEFAULT_REF_TEMPLATE`.
-            schema_generator (Type[GenerateJsonSchema]): The JSON schema generator. Defaults to `GenerateJsonSchema`.
+            by_alias: Whether to use attribute aliases or not. Defaults to `True`.
+            ref_template: The reference template. Defaults to `DEFAULT_REF_TEMPLATE`.
+            schema_generator: The JSON schema generator. Defaults to `GenerateJsonSchema`.
 
         Returns:
-            Dict: The JSON schema for the given `cls` model class.
+            The JSON schema for the given `cls` model class.
         """
         return model_json_schema(
             cls, by_alias=by_alias, ref_template=ref_template, schema_generator=schema_generator, mode=mode
         )
 
     @classmethod
     def model_rebuild(
@@ -541,25 +546,24 @@
         *,
         force: bool = False,
         raise_errors: bool = True,
         _parent_namespace_depth: int = 2,
         _types_namespace: dict[str, Any] | None = None,
     ) -> bool | None:
         """
-        Try to rebuild or reconstruct the model core schema
+        Tries to rebuild or reconstruct the model core schema.
 
         Args:
-            cls (type): The class to build the model core schema for.
-            force (bool): Whether to force the rebuilding of the model schema, defaults to `False`.
-            raise_errors (bool): Whether to raise errors, defaults to `True`.
-            _parent_namespace_depth (int): The depth level of the parent namespace, defaults to 2.
-            _types_namespace (dict[str, Any] | None): The types namespace, defaults to `None`.
+            force: Whether to force the rebuilding of the model schema, defaults to `False`.
+            raise_errors: Whether to raise errors, defaults to `True`.
+            _parent_namespace_depth: The depth level of the parent namespace, defaults to 2.
+            _types_namespace: The types namespace, defaults to `None`.
 
         Returns:
-            bool or None: Returns `None` if model schema is complete and no rebuilding is required.
+            Returns `None` if model schema is complete and no rebuilding is required.
                 If rebuilding _is_ required, returns `True` if rebuilding was successful, otherwise `False`.
         """
         if not force and cls.__pydantic_complete__:
             return None
         else:
             if _types_namespace is not None:
                 types_namespace: dict[str, Any] | None = _types_namespace.copy()
@@ -601,23 +605,23 @@
                 and self.__pydantic_extra__ == other.__pydantic_extra__
             )
         else:
             return NotImplemented  # delegate to the other item in the comparison
 
     def model_copy(self: Model, *, update: dict[str, Any] | None = None, deep: bool = False) -> Model:
         """
-        Returns a copy of the Model.
+        Returns a copy of the model.
 
         Args:
-            update (Optional[Dict[str, Any]]): Values to change/add in the new model. Note: the data is not validated
+            update: Values to change/add in the new model. Note: the data is not validated
                 before creating the new model. You should trust this data.
-            deep (bool): Set to `True` to make a deep copy of the model.
+            deep: Set to `True` to make a deep copy of the model.
 
         Returns:
-            Model: New model instance.
+            New model instance.
         """
         copied = self.__deepcopy__() if deep else self.__copy__()
         if update:
             if self.model_config.get('extra') == 'allow':
                 for k, v in update.items():
                     if k in self.model_fields:
                         copied.__dict__[k] = v
@@ -693,15 +697,15 @@
         return self.__repr_str__(' ')
 
     def __repr__(self) -> str:
         return f'{self.__repr_name__()}({self.__repr_str__(", ")})'
 
     def __class_getitem__(
         cls, typevar_values: type[Any] | tuple[type[Any], ...]
-    ) -> type[BaseModel] | _forward_ref.PydanticForwardRef | _forward_ref.PydanticRecursiveRef:
+    ) -> type[BaseModel] | _forward_ref.PydanticRecursiveRef:
         cached = _generics.get_cached_generic_type_early(cls, typevar_values)
         if cached is not None:
             return cached
 
         if cls is BaseModel:
             raise TypeError('Type parameters should be placed on typing.Generic, not BaseModel')
         if not hasattr(cls, '__parameters__'):
@@ -758,25 +762,25 @@
                 _generics.set_cached_generic_type(cls, typevar_values, submodel, origin, args)
 
         return submodel
 
     @classmethod
     def model_parametrized_name(cls, params: tuple[type[Any], ...]) -> str:
         """
-        Compute class name for parametrizations of generic classes.
+        Compute the class name for parametrizations of generic classes.
 
         This method can be overridden to achieve a custom naming scheme for generic BaseModels.
 
         Args:
-            params (tuple[type[Any], ...]): Tuple of types of the class. Given a generic class
+            params: Tuple of types of the class. Given a generic class
                 `Model` with 2 type variables and a concrete model `Model[str, int]`,
                 the value `(str, int)` would be passed to `params`.
 
         Returns:
-            str: String representing the new class where `params` are passed to `cls` as type variables.
+            String representing the new class where `params` are passed to `cls` as type variables.
 
         Raises:
             TypeError: Raised when trying to generate concrete names for non-generic models.
         """
         if not issubclass(cls, typing.Generic):  # type: ignore[arg-type]
             raise TypeError('Concrete names should only be generated for generic models.')
 
@@ -966,19 +970,38 @@
         *,
         include: AbstractSetIntStr | MappingIntStrAny | None = None,
         exclude: AbstractSetIntStr | MappingIntStrAny | None = None,
         update: typing.Dict[str, Any] | None = None,  # noqa UP006
         deep: bool = False,
     ) -> Model:  # pragma: no cover
         """
-        This method is now deprecated; use `model_copy` instead. If you need include / exclude, use:
+        Returns a copy of the model.
 
-            data = self.model_dump(include=include, exclude=exclude, round_trip=True)
-            data = {**data, **(update or {})}
-            copied = self.model_validate(data)
+        This method is now deprecated; use `model_copy` instead. If you need `include` or `exclude`, use:
+
+        ```py
+        data = self.model_dump(include=include, exclude=exclude, round_trip=True)
+        data = {**data, **(update or {})}
+        copied = self.model_validate(data)
+        ```
+
+        Args:
+            include: Optional set or mapping
+                specifying which fields to include in the copied model.
+            exclude: Optional set or mapping
+                specifying which fields to exclude in the copied model.
+            update: Optional dictionary of field-value pairs to override field values
+                in the copied model.
+            deep: If True, the values of fields that are Pydantic models will be deep copied.
+
+        Returns:
+            A copy of the model with included, excluded and updated fields as specified.
+
+        Raises:
+            DeprecationWarning: The `copy` method is deprecated; use `model_copy` instead.
         """
         warnings.warn(
             'The `copy` method is deprecated; use `model_copy` instead. '
             'See the docstring of `BaseModel.copy` for details about how to handle `include` and `exclude`.',
             DeprecationWarning,
         )
 
@@ -1092,14 +1115,21 @@
         return _deprecated_copy_internals._calculate_keys(self, *args, **kwargs)  # type: ignore
 
 
 RootModelRootType = typing.TypeVar('RootModelRootType')
 
 
 class RootModel(BaseModel, typing.Generic[RootModelRootType]):
+    """
+    A Pydantic `BaseModel` for the root object of the model.
+
+    Attributes:
+        root (RootModelRootType): The root object of the model.
+    """
+
     __pydantic_root_model__ = True
     # TODO: Make `__pydantic_fields_set__` logic consistent with `BaseModel`, i.e. it should be `set()` if default value
     # was used
     __pydantic_fields_set__ = {'root'}  # It's fine having a set here as it will never change
     __pydantic_private__ = None
     __pydantic_extra__ = None
 
@@ -1109,14 +1139,27 @@
         __tracebackhide__ = True
         __pydantic_self__.__pydantic_validator__.validate_python(root, self_instance=__pydantic_self__)
 
     __init__.__pydantic_base_init__ = True  # type: ignore
 
     @classmethod
     def model_construct(cls: type[Model], root: RootModelRootType, _fields_set: set[str] | None = None) -> Model:
+        """
+        Create a new model using the provided root object and update fields set.
+
+        Args:
+            root: The root object of the model.
+            _fields_set: The set of fields to be updated.
+
+        Returns:
+            The new model.
+
+        Raises:
+            NotImplemented: If the model is not a subclass of `RootModel`.
+        """
         return super().model_construct(root=root, _fields_set=_fields_set)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, RootModel):
             return NotImplemented
         return self.model_fields['root'].annotation == other.model_fields['root'].annotation and super().__eq__(other)
 
@@ -1160,31 +1203,34 @@
     __module__: str = __name__,
     __validators__: dict[str, AnyClassMethod] | None = None,
     __cls_kwargs__: dict[str, Any] | None = None,
     __slots__: tuple[str, ...] | None = None,
     **field_definitions: Any,
 ) -> type[Model]:
     """
-    Dynamically creates and returns a new Pydantic Model.
+    Dynamically creates and returns a new Pydantic model.
 
     Args:
-        __model_name (str): The name of the newly created model.
-        __config__ (Optional[ConfigDict]): The configuration of the new model.
-        __base__ (Optional[Union[type[Model], Tuple[type[Model]]]]): The base class for the new model.
-        __module__ (str): The name of the module that the model belongs to.
-        __validators__ (Optional[Dict[str, Union[Callable, ClassMethod]]]): A dictionary of methods that validate
+        __model_name: The name of the newly created model.
+        __config__: The configuration of the new model.
+        __base__: The base class for the new model.
+        __module__: The name of the module that the model belongs to.
+        __validators__: A dictionary of methods that validate
             fields.
-        __cls_kwargs__ (Optional[Dict[str, Any]]): A dictionary of keyword arguments for class creation.
-        __slots__ (Optional[Tuple[str]]): Deprecated. Should not be passed to `create_model`.
-        **field_definitions (Any): Attributes of the new model. They should be passed in the format:
+        __cls_kwargs__: A dictionary of keyword arguments for class creation.
+        __slots__: Deprecated. Should not be passed to `create_model`.
+        **field_definitions: Attributes of the new model. They should be passed in the format:
             `<name>=(<type>, <default value>)` or `<name>=<default value>`. For more complex cases, they can be
             passed in the format: `<name>=<Field>` or `<name>=(<type>, <FieldInfo>)`.
 
     Returns:
-        Model: The newly created Pydantic Model.
+        The newly created model.
+
+    Raises:
+        PydanticUserError: If `__base__` and `__config__` are both passed.
     """
     if __slots__ is not None:
         # __slots__ will be ignored from here on
         warnings.warn('__slots__ should not be passed to create_model', RuntimeWarning)
 
     if __base__ is not None:
         if __config__ is not None:
```

### Comparing `pydantic-2.0b1/pydantic/mypy.py` & `pydantic-2.0b2/pydantic/mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/networks.py` & `pydantic-2.0b2/pydantic/networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/type_adapter.py` & `pydantic-2.0b2/pydantic/type_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -162,28 +162,36 @@
         except AttributeError:
             serializer = SchemaSerializer(simplified_core_schema, core_config)
 
         self.core_schema = core_schema
         self.validator = validator
         self.serializer = serializer
 
-    def validate_python(self, __object: Any, *, strict: bool | None = None, context: dict[str, Any] | None = None) -> T:
+    def validate_python(
+        self,
+        __object: Any,
+        *,
+        strict: bool | None = None,
+        from_attributes: bool | None = None,
+        context: dict[str, Any] | None = None,
+    ) -> T:
         """
         Validate a Python object against the model.
 
         Args:
             __object (Any): The Python object to validate against the model.
             strict (bool | None, optional): Whether to strictly check types. Defaults to None.
+            from_attributes (bool | None, optional): Whether to extract data from object attributes. Defaults to None.
             context (dict[str, Any] | None, optional): Additional context to use during validation. Defaults to None.
 
         Returns:
             T: The validated object.
 
         """
-        return self.validator.validate_python(__object, strict=strict, context=context)
+        return self.validator.validate_python(__object, strict=strict, from_attributes=from_attributes, context=context)
 
     def validate_json(
         self, __data: str | bytes, *, strict: bool | None = None, context: dict[str, Any] | None = None
     ) -> T:
         """Validate a JSON string or bytes against the model.
 
         Args:
```

### Comparing `pydantic-2.0b1/pydantic/types.py` & `pydantic-2.0b2/pydantic/types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/validate_call.py` & `pydantic-2.0b2/pydantic/validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/version.py` & `pydantic-2.0b2/pydantic/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = 'VERSION', 'version_info'
 
-VERSION = '2.0b1'
+VERSION = '2.0b2'
 
 
 def version_info() -> str:
     import platform
     import sys
     from importlib import import_module
     from pathlib import Path
```

### Comparing `pydantic-2.0b1/pydantic/_internal/_annotated_handlers.py` & `pydantic-2.0b2/pydantic/_internal/_annotated_handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_config.py` & `pydantic-2.0b2/pydantic/_internal/_config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_core_metadata.py` & `pydantic-2.0b2/pydantic/_internal/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_core_utils.py` & `pydantic-2.0b2/pydantic/_internal/_core_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_dataclasses.py` & `pydantic-2.0b2/pydantic/_internal/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_decorators.py` & `pydantic-2.0b2/pydantic/_internal/_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_decorators_v1.py` & `pydantic-2.0b2/pydantic/_internal/_decorators_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_discriminated_union.py` & `pydantic-2.0b2/pydantic/_internal/_discriminated_union.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_fields.py` & `pydantic-2.0b2/pydantic/_internal/_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import dataclasses
 import sys
 from copy import copy
 from typing import TYPE_CHECKING, Any
 
 from . import _typing_extra
 from ._config import ConfigWrapper
-from ._forward_ref import PydanticForwardRef
 from ._repr import Representation
 from ._typing_extra import get_cls_type_hints_lenient, get_type_hints, is_classvar, is_finalvar
 
 if TYPE_CHECKING:
     from ..fields import FieldInfo
     from ..main import BaseModel
     from ._dataclasses import StandardDataclass
@@ -132,16 +131,14 @@
         try:
             default = getattr(cls, ann_name, Undefined)
             if default is Undefined:
                 raise AttributeError
         except AttributeError:
             if ann_name in annotations:
                 field_info = FieldInfo.from_annotation(ann_type)
-            elif isinstance(ann_type, PydanticForwardRef):
-                field_info = FieldInfo.from_annotation(annotation=ann_type)  # type: ignore
             else:
                 # if field has no default value and is not in __annotations__ this means that it is
                 # defined in a base class and we can take it from there
                 model_fields_lookup: dict[str, FieldInfo] = {}
                 for x in cls.__bases__[::-1]:
                     model_fields_lookup.update(getattr(x, 'model_fields', {}))
                 if ann_name in model_fields_lookup:
```

### Comparing `pydantic-2.0b1/pydantic/_internal/_generate_schema.py` & `pydantic-2.0b2/pydantic/_internal/_generate_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import collections.abc
 import dataclasses
 import inspect
 import re
 import sys
 import typing
-import warnings
 from functools import partial
 from inspect import Parameter, _ParameterKind, signature
 from itertools import chain
 from operator import attrgetter
 from types import FunctionType, LambdaType, MethodType
 from typing import TYPE_CHECKING, Any, Callable, ForwardRef, Iterable, Mapping, TypeVar, Union, cast
 
@@ -54,15 +53,15 @@
     inspect_validator,
 )
 from ._fields import (
     Undefined,
     collect_dataclass_fields,
     get_type_hints_infer_globalns,
 )
-from ._forward_ref import PydanticForwardRef, PydanticRecursiveRef
+from ._forward_ref import PydanticRecursiveRef
 from ._generics import get_standard_typevars_map, recursively_defined_type_refs, replace_types
 from ._schema_generation_shared import (
     CallbackGetCoreSchemaHandler,
     UnpackedRefJsonSchemaHandler,
     wrap_json_schema_fn_for_model_or_custom_type_with_ref_unpacking,
 )
 from ._typing_extra import is_finalvar
@@ -381,30 +380,14 @@
 
         if lenient_issubclass(obj, BaseModel):
             return self.model_schema(obj)
 
         if isinstance(obj, PydanticRecursiveRef):
             return core_schema.definition_reference_schema(schema_ref=obj.type_ref)
 
-        if isinstance(obj, PydanticForwardRef):
-            if not obj.deferred_actions:
-                return obj.schema
-            resolved_model = obj.resolve_model()
-            if isinstance(resolved_model, PydanticForwardRef):
-                # If you still have a PydanticForwardRef after resolving, it should be deeply nested enough that it will
-                # eventually be substituted out. So it is safe to return an invalid schema here.
-                # TODO: Replace this with a (new) CoreSchema that, if present at any level, makes validation fail
-                #   Issue: https://github.com/pydantic/pydantic-core/issues/619
-                return core_schema.none_schema(
-                    metadata={'invalid': True, 'pydantic_debug_self_schema': resolved_model.schema}
-                )
-            else:
-                model_ref = get_type_ref(resolved_model)
-                return core_schema.definition_reference_schema(model_ref)
-
         try:
             if obj in {bool, int, float, str, bytes, list, set, frozenset, dict}:
                 # Note: obj may fail to be hashable if it has an unhashable annotation
                 return {'type': obj.__name__}
             elif obj is tuple:
                 return {'type': 'tuple-variable'}
         except TypeError:  # obj not hashable; can happen due to unhashable annotations
@@ -825,32 +808,35 @@
 
     def _tuple_schema(self, tuple_type: Any) -> core_schema.CoreSchema:
         """
         Generate schema for a Tuple, e.g. `tuple[int, str]` or `tuple[int, ...]`.
         """
         params = get_args(tuple_type)
         # NOTE: subtle difference: `tuple[()]` gives `params=()`, whereas `typing.Tuple[()]` gives `params=((),)`
+        # This is only true for <3.11, on Python 3.11+ `typing.Tuple[()]` gives `params=()`
         if not params:
             if tuple_type == typing.Tuple:
                 return core_schema.tuple_variable_schema()
             else:
                 # special case for `tuple[()]` which means `tuple[]` - an empty tuple
                 return core_schema.tuple_positional_schema([])
         elif params[-1] is Ellipsis:
             if len(params) == 2:
                 sv = core_schema.tuple_variable_schema(self.generate_schema(params[0]))
                 return sv
 
-            # not sure this case is valid in python, but may as well support it here since pydantic-core does
-            *items_schema, extra_schema = params
-            return core_schema.tuple_positional_schema(
+            # NOTE: This is not valid in Python, but not removing it because it's
+            # going to be useful for https://github.com/pydantic/pydantic/issues/5952
+            *items_schema, extra_schema = params  # pragma: no cover
+            return core_schema.tuple_positional_schema(  # pragma: no cover
                 [self.generate_schema(p) for p in items_schema], extra_schema=self.generate_schema(extra_schema)
             )
         elif len(params) == 1 and params[0] == ():
             # special case for `Tuple[()]` which means `Tuple[]` - an empty tuple
+            # NOTE: This conditional can be removed when we drop support for Python 3.10.
             return core_schema.tuple_positional_schema([])
         else:
             return core_schema.tuple_positional_schema([self.generate_schema(p) for p in params])
 
     def _type_schema(self) -> core_schema.CoreSchema:
         return core_schema.custom_error_schema(
             core_schema.is_instance_schema(type),
@@ -1457,20 +1443,20 @@
         return Any
 
 
 def _extract_get_pydantic_json_schema(tp: Any, schema: CoreSchema) -> GetJsonSchemaFunction | None:
     """Extract `__get_pydantic_json_schema__` from a type, handling the deprecated `__modify_schema__`"""
     js_modify_function = getattr(tp, '__get_pydantic_json_schema__', None)
 
-    if js_modify_function is None and hasattr(tp, '__modify_schema__'):
-        warnings.warn(
-            'The __modify_schema__ method is deprecated, use __get_pydantic_json_schema__ instead',
-            DeprecationWarning,
+    if hasattr(tp, '__modify_schema__'):
+        raise PydanticUserError(
+            'The `__modify_schema__` method is not supported in Pydantic v2. '
+            'Use `__get_pydantic_json_schema__` instead.',
+            code='custom-json-schema',
         )
-        return lambda c, h: tp.__modify_schema__(h(c))
 
     # handle GenericAlias' but ignore Annotated which "lies" about it's origin (in this case it would be `int`)
     if hasattr(tp, '__origin__') and not isinstance(tp, type(Annotated[int, 'placeholder'])):
         return _extract_get_pydantic_json_schema(tp.__origin__, schema)
 
     if js_modify_function is None:
         return None
```

### Comparing `pydantic-2.0b1/pydantic/_internal/_generics.py` & `pydantic-2.0b2/pydantic/_internal/_generics.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from types import prepare_class
 from typing import TYPE_CHECKING, Any, Iterator, List, Mapping, MutableMapping, Tuple, TypeVar
 from weakref import WeakValueDictionary
 
 import typing_extensions
 
 from ._core_utils import get_type_ref
-from ._forward_ref import PydanticForwardRef, PydanticRecursiveRef
+from ._forward_ref import PydanticRecursiveRef
 from ._typing_extra import TypeVarType, typing_base
 from ._utils import all_identical, is_basemodel
 
 if sys.version_info >= (3, 10):
     from typing import _UnionGenericAlias  # type: ignore[attr-defined]
 
 if TYPE_CHECKING:
@@ -312,18 +312,14 @@
     # `typing.Callable[[int, str], int]` is an example for this.
     if isinstance(type_, (List, list)):
         resolved_list = list(replace_types(element, type_map) for element in type_)
         if all_identical(type_, resolved_list):
             return type_
         return resolved_list
 
-    if isinstance(type_, PydanticForwardRef):
-        # queue the replacement as a deferred action
-        return type_.replace_types(type_map)
-
     # If all else fails, we try to resolve the type directly and otherwise just
     # return the input with no modifications.
     return type_map.get(type_, type_)
 
 
 def check_parameters_count(cls: type[BaseModel], parameters: tuple[Any, ...]) -> None:
     actual = len(parameters)
@@ -335,15 +331,15 @@
 
 _generic_recursion_cache: ContextVar[set[str] | None] = ContextVar('_generic_recursion_cache', default=None)
 
 
 @contextmanager
 def generic_recursion_self_type(
     origin: type[BaseModel], args: tuple[Any, ...]
-) -> Iterator[PydanticForwardRef | PydanticRecursiveRef | None]:
+) -> Iterator[PydanticRecursiveRef | None]:
     """
     This contextmanager should be placed around the recursive calls used to build a generic type,
     and accept as arguments the generic origin type and the type arguments being passed to it.
 
     If the same origin and arguments are observed twice, it implies that a self-reference placeholder
     can be used while building the core schema, and will produce a schema_ref that will be valid in the
     final parent schema.
```

### Comparing `pydantic-2.0b1/pydantic/_internal/_known_annotated_metadata.py` & `pydantic-2.0b2/pydantic/_internal/_known_annotated_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_model_construction.py` & `pydantic-2.0b2/pydantic/_internal/_model_construction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_repr.py` & `pydantic-2.0b2/pydantic/_internal/_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_schema_generation_shared.py` & `pydantic-2.0b2/pydantic/_internal/_schema_generation_shared.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_std_types_schema.py` & `pydantic-2.0b2/pydantic/_internal/_std_types_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_typing_extra.py` & `pydantic-2.0b2/pydantic/_internal/_typing_extra.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_utils.py` & `pydantic-2.0b2/pydantic/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_validate_call.py` & `pydantic-2.0b2/pydantic/_internal/_validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/_internal/_validators.py` & `pydantic-2.0b2/pydantic/_internal/_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/deprecated/class_validators.py` & `pydantic-2.0b2/pydantic/deprecated/class_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/deprecated/config.py` & `pydantic-2.0b2/pydantic/deprecated/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/deprecated/copy_internals.py` & `pydantic-2.0b2/pydantic/deprecated/copy_internals.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/deprecated/decorator.py` & `pydantic-2.0b2/pydantic/deprecated/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/deprecated/json.py` & `pydantic-2.0b2/pydantic/deprecated/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/deprecated/parse.py` & `pydantic-2.0b2/pydantic/deprecated/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/deprecated/tools.py` & `pydantic-2.0b2/pydantic/deprecated/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/__init__.py` & `pydantic-2.0b2/pydantic/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/_hypothesis_plugin.py` & `pydantic-2.0b2/pydantic/v1/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/annotated_types.py` & `pydantic-2.0b2/pydantic/v1/annotated_types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/class_validators.py` & `pydantic-2.0b2/pydantic/v1/class_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/color.py` & `pydantic-2.0b2/pydantic/v1/color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/config.py` & `pydantic-2.0b2/pydantic/v1/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/dataclasses.py` & `pydantic-2.0b2/pydantic/v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/datetime_parse.py` & `pydantic-2.0b2/pydantic/v1/datetime_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/decorator.py` & `pydantic-2.0b2/pydantic/v1/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/env_settings.py` & `pydantic-2.0b2/pydantic/v1/env_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/error_wrappers.py` & `pydantic-2.0b2/pydantic/v1/error_wrappers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/errors.py` & `pydantic-2.0b2/pydantic/v1/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/fields.py` & `pydantic-2.0b2/pydantic/v1/fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/generics.py` & `pydantic-2.0b2/pydantic/v1/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/json.py` & `pydantic-2.0b2/pydantic/v1/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/main.py` & `pydantic-2.0b2/pydantic/v1/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/mypy.py` & `pydantic-2.0b2/pydantic/v1/mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/networks.py` & `pydantic-2.0b2/pydantic/v1/networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/parse.py` & `pydantic-2.0b2/pydantic/v1/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/schema.py` & `pydantic-2.0b2/pydantic/v1/schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/tools.py` & `pydantic-2.0b2/pydantic/v1/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/types.py` & `pydantic-2.0b2/pydantic/v1/types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/typing.py` & `pydantic-2.0b2/pydantic/v1/typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/utils.py` & `pydantic-2.0b2/pydantic/v1/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/validators.py` & `pydantic-2.0b2/pydantic/v1/validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pydantic/v1/version.py` & `pydantic-2.0b2/pydantic/v1/version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/conftest.py` & `pydantic-2.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_abc.py` & `pydantic-2.0b2/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_aliases.py` & `pydantic-2.0b2/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_annotated.py` & `pydantic-2.0b2/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_assert_in_validators.py` & `pydantic-2.0b2/tests/test_assert_in_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_callable.py` & `pydantic-2.0b2/tests/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_color.py` & `pydantic-2.0b2/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_computed_fields.py` & `pydantic-2.0b2/tests/test_computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_config.py` & `pydantic-2.0b2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_construction.py` & `pydantic-2.0b2/tests/test_construction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_create_model.py` & `pydantic-2.0b2/tests/test_create_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import platform
-from typing import Optional, Tuple
+from typing import Generic, Optional, Tuple, TypeVar
 
 import pytest
 
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
@@ -63,14 +63,24 @@
         m2 = pickle.loads(d)
         assert m2.foo == m.foo == 'hello'
         assert m2.bar == m.bar == 123
         assert m2 == m
         assert m2 is not m
 
 
+def test_create_model_multi_inheritance():
+    class Mixin:
+        pass
+
+    Generic_T = Generic[TypeVar('T')]
+    FooModel = create_model('FooModel', value=(int, ...), __base__=(BaseModel, Generic_T))
+
+    assert FooModel.__orig_bases__ == (BaseModel, Generic_T)
+
+
 def test_invalid_name():
     with pytest.warns(RuntimeWarning):
         model = create_model('FooModel', _foo=(str, ...))
     assert len(model.model_fields) == 0
 
 
 def test_field_wrong_tuple():
```

### Comparing `pydantic-2.0b1/tests/test_dataclasses.py` & `pydantic-2.0b2/tests/test_dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing_extensions import Literal
 
 import pydantic
 from pydantic import (
     BaseModel,
     ConfigDict,
     FieldValidationInfo,
+    PydanticUndefinedAnnotation,
     PydanticUserError,
     TypeAdapter,
     ValidationError,
     computed_field,
     field_serializer,
     field_validator,
     model_validator,
@@ -2290,7 +2291,22 @@
         z2: ClassVar[str] = 'z2-classvar'
 
     dc = TypeAdapter(SubModel).validate_python({'x': 1, 'y': 'a', 'x2': 2, 'y2': 'b'})
     assert dc.x == 1
     assert dc.x2 == 2
     assert SubModel.z == 'z-classvar'
     assert SubModel.z2 == 'z2-classvar'
+
+
+def test_rebuild_dataclass():
+    @pydantic.dataclasses.dataclass
+    class MyDataClass:
+        x: str
+
+    assert rebuild_dataclass(MyDataClass) is None
+
+    @pydantic.dataclasses.dataclass()
+    class MyDataClass1:
+        d2: Optional['Foo'] = None  # noqa F821
+
+    with pytest.raises(PydanticUndefinedAnnotation, match="name 'Foo' is not defined"):
+        rebuild_dataclass(MyDataClass1, _parent_namespace_depth=0)
```

### Comparing `pydantic-2.0b1/tests/test_datetime.py` & `pydantic-2.0b2/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_decorators.py` & `pydantic-2.0b2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_deprecated.py` & `pydantic-2.0b2/tests/test_deprecated.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,14 +452,28 @@
 def test_field_regex():
     with pytest.raises(PydanticUserError, match='`regex` is removed. use `pattern` instead'):
 
         class Model(BaseModel):
             x: str = Field('test', regex=r'^test$')
 
 
+def test_modify_schema_error():
+    with pytest.raises(
+        PydanticUserError,
+        match='The `__modify_schema__` method is not supported in Pydantic v2. '
+        'Use `__get_pydantic_json_schema__` instead.',
+    ):
+
+        class Model(BaseModel):
+            def __modify_schema__(self, field_schema: Dict[str, Any]) -> None:
+                pass
+
+        Model()
+
+
 def test_field_extra_arguments():
     m = 'Extra keyword arguments on `Field` is deprecated and will be removed. use `json_schema_extra` instead'
     with pytest.warns(DeprecationWarning, match=m):
 
         class Model(BaseModel):
             x: str = Field('test', test='test')
```

### Comparing `pydantic-2.0b1/tests/test_deprecated_validate_arguments.py` & `pydantic-2.0b2/tests/test_deprecated_validate_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_discriminated_union.py` & `pydantic-2.0b2/tests/test_discriminated_union.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_docs.py` & `pydantic-2.0b2/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_edge_cases.py` & `pydantic-2.0b2/tests/test_edge_cases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_errors.py` & `pydantic-2.0b2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_exports.py` & `pydantic-2.0b2/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_fastapi_json_schema.py` & `pydantic-2.0b2/tests/test_fastapi_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_fields.py` & `pydantic-2.0b2/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_forward_ref.py` & `pydantic-2.0b2/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_generics.py` & `pydantic-2.0b2/tests/test_generics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1437,14 +1437,45 @@
 
     class ReferenceModel(BaseModel, Generic[T]):
         abstract_base_with_type: ModelWithType[T]
 
     ReferenceModel[int]
 
 
+def test_generic_with_referenced_generic_type_bound():
+    T = TypeVar('T', bound=int)
+
+    class ModelWithType(BaseModel, Generic[T]):
+        # Type resolves to type origin of "type" which is non-subscriptible for
+        # python < 3.9 so we want to make sure it works for other versions
+        some_type: Type[T]
+
+    class ReferenceModel(BaseModel, Generic[T]):
+        abstract_base_with_type: ModelWithType[T]
+
+    class MyInt(int):
+        ...
+
+    ReferenceModel[MyInt]
+
+
+def test_generic_with_referenced_generic_type_constraints():
+    T = TypeVar('T', int, str)
+
+    class ModelWithType(BaseModel, Generic[T]):
+        # Type resolves to type origin of "type" which is non-subscriptible for
+        # python < 3.9 so we want to make sure it works for other versions
+        some_type: Type[T]
+
+    class ReferenceModel(BaseModel, Generic[T]):
+        abstract_base_with_type: ModelWithType[T]
+
+    ReferenceModel[int]
+
+
 def test_generic_with_referenced_nested_typevar():
     T = TypeVar('T')
 
     class ModelWithType(BaseModel, Generic[T]):
         # Type resolves to type origin of "collections.abc.Sequence" which is
         # non-subscriptible for
         # python < 3.9 so we want to make sure it works for other versions
```

### Comparing `pydantic-2.0b1/tests/test_internal.py` & `pydantic-2.0b2/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_json.py` & `pydantic-2.0b2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_json_schema.py` & `pydantic-2.0b2/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_main.py` & `pydantic-2.0b2/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import platform
 import re
 import sys
 from copy import deepcopy
+from dataclasses import dataclass
 from enum import Enum
 from typing import (
     Any,
     Callable,
     ClassVar,
     Dict,
     Generic,
@@ -1881,29 +1882,45 @@
 
 
 def test_model_rebuild_localns():
     class A(BaseModel):
         x: int
 
     class B(BaseModel):
-        a: 'Model'  # noqa F821
+        a: 'Model'  # noqa: F821
 
     B.model_rebuild(_types_namespace={'Model': A})
 
     m = B(a={'x': 1})
     assert m.model_dump() == {'a': {'x': 1}}
     assert isinstance(m.a, A)
 
     class C(BaseModel):
-        a: 'Model'  # noqa F821
+        a: 'Model'  # noqa: F821
 
     with pytest.raises(PydanticUndefinedAnnotation, match="name 'Model' is not defined"):
         C.model_rebuild(_types_namespace={'A': A})
 
 
+def test_model_rebuild_zero_depth():
+    class Model(BaseModel):
+        x: 'X_Type'
+
+    X_Type = str
+
+    with pytest.raises(NameError, match='X_Type'):
+        Model.model_rebuild(_parent_namespace_depth=0)
+
+    Model.__pydantic_parent_namespace__.update({'X_Type': int})
+    Model.model_rebuild(_parent_namespace_depth=0)
+
+    m = Model(x=42)
+    assert m.model_dump() == {'x': 42}
+
+
 @pytest.fixture(scope='session', name='InnerEqualityModel')
 def inner_equality_fixture():
     class InnerEqualityModel(BaseModel):
         iw: int
         ix: int = 0
         _iy: int = PrivateAttr()
         _iz: int = PrivateAttr(0)
@@ -1998,19 +2015,24 @@
     assert m2.model_dump() == {'x': 1, 'y': 2}
     assert m2.model_extra == {'y': 2}
 
     m3 = m.model_copy(update={'x': 4, 'z': 3})
     assert m3.model_dump() == {'x': 4, 'y': 2, 'z': 3}
     assert m3.model_extra == {'y': 2, 'z': 3}
 
-    m3.__pydantic_extra__ = None
     m4 = m.model_copy(update={'x': 4, 'z': 3})
     assert m4.model_dump() == {'x': 4, 'y': 2, 'z': 3}
     assert m4.model_extra == {'y': 2, 'z': 3}
 
+    m = Model(x=1, a=2)
+    m.__pydantic_extra__ = None
+    m5 = m.model_copy(update={'x': 4, 'b': 3})
+    assert m5.model_dump() == {'x': 4, 'b': 3}
+    assert m5.model_extra == {'b': 3}
+
 
 def test_model_parametrized_name_not_generic():
     class Model(BaseModel):
         x: int
 
     with pytest.raises(TypeError, match='Concrete names should only be generated for generic models.'):
         Model.model_parametrized_name(())
@@ -2279,7 +2301,54 @@
     assert GoodModel.MyType is NonNestedType
     assert GoodModel.x is GoodModel.NestedType
 
     with pytest.raises(PydanticUserError, match='A non-annotated attribute was detected'):
 
         class BadModel(BaseModel):
             x = NonNestedType
+
+
+def test_validate_python_from_attributes() -> None:
+    class Model(BaseModel):
+        x: int
+
+    class ModelFromAttributesTrue(Model):
+        model_config = ConfigDict(from_attributes=True)
+
+    class ModelFromAttributesFalse(Model):
+        model_config = ConfigDict(from_attributes=False)
+
+    @dataclass
+    class UnrelatedClass:
+        x: int = 1
+
+    input = UnrelatedClass(1)
+
+    for from_attributes in (False, None):
+        with pytest.raises(ValidationError) as exc_info:
+            Model.model_validate(UnrelatedClass(), from_attributes=from_attributes)
+        assert exc_info.value.errors(include_url=False) == [
+            {'type': 'dict_type', 'loc': (), 'msg': 'Input should be a valid dictionary', 'input': input}
+        ]
+
+    res = Model.model_validate(UnrelatedClass(), from_attributes=True)
+    assert res == Model(x=1)
+
+    with pytest.raises(ValidationError) as exc_info:
+        ModelFromAttributesTrue.model_validate(UnrelatedClass(), from_attributes=False)
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'dict_type', 'loc': (), 'msg': 'Input should be a valid dictionary', 'input': input}
+    ]
+
+    for from_attributes in (True, None):
+        res = ModelFromAttributesTrue.model_validate(UnrelatedClass(), from_attributes=from_attributes)
+        assert res == ModelFromAttributesTrue(x=1)
+
+    for from_attributes in (False, None):
+        with pytest.raises(ValidationError) as exc_info:
+            ModelFromAttributesFalse.model_validate(UnrelatedClass(), from_attributes=from_attributes)
+        assert exc_info.value.errors(include_url=False) == [
+            {'type': 'dict_type', 'loc': (), 'msg': 'Input should be a valid dictionary', 'input': input}
+        ]
+
+    res = ModelFromAttributesFalse.model_validate(UnrelatedClass(), from_attributes=True)
+    assert res == ModelFromAttributesFalse(x=1)
```

### Comparing `pydantic-2.0b1/tests/test_migration.py` & `pydantic-2.0b2/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_model_signature.py` & `pydantic-2.0b2/tests/test_model_signature.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_model_validator.py` & `pydantic-2.0b2/tests/test_model_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 from __future__ import annotations
 
-from pprint import pprint
 from typing import Any, Dict, Union, cast
 
 import pytest
 
-from pydantic import BaseModel, ValidationInfo, model_validator
+from pydantic import BaseModel, ValidationInfo, ValidatorFunctionWrapHandler, model_validator
 
 
 def test_model_validator_wrap() -> None:
     class Model(BaseModel):
         x: int
         y: int
 
         @model_validator(mode='wrap')
         @classmethod
-        def val_model(cls, values, handler, info) -> Model:
-            return handler(values)
+        def val_model(cls, values: dict[str, Any] | Model, handler: ValidatorFunctionWrapHandler) -> Model:
+            if isinstance(values, dict):
+                assert values == {'x': 1, 'y': 2}
+                model = handler({'x': 2, 'y': 3})
+            else:
+                assert values.x == 1
+                assert values.y == 2
+                model = handler(Model.model_construct(x=2, y=3))
+            assert model.x == 2
+            assert model.y == 3
+            model.x = 20
+            model.y = 30
+            return model
 
-    pprint(Model.__pydantic_core_schema__)
-    # Model(x=1, y=2).model_dump()
-    # assert Model.model_validate(Model(x=1, y=2)).model_dump() == {'x': 3, 'y': 4}
+    assert Model(x=1, y=2).model_dump() == {'x': 20, 'y': 30}
+    assert Model.model_validate(Model.model_construct(x=1, y=2)).model_dump() == {'x': 20, 'y': 30}
 
 
 @pytest.mark.parametrize('classmethod_decorator', [classmethod, lambda x: x])
 def test_model_validator_before(classmethod_decorator: Any) -> None:
     class Model(BaseModel):
         x: int
         y: int
```

### Comparing `pydantic-2.0b1/tests/test_networks.py` & `pydantic-2.0b2/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_networks_ipaddress.py` & `pydantic-2.0b2/tests/test_networks_ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_parse.py` & `pydantic-2.0b2/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_prepare_annotations.py` & `pydantic-2.0b2/tests/test_prepare_annotations.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_private_attributes.py` & `pydantic-2.0b2/tests/test_private_attributes.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_rich_repr.py` & `pydantic-2.0b2/tests/test_rich_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_root_model.py` & `pydantic-2.0b2/tests/test_root_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,14 +312,25 @@
 def test_root_model_nested_equality():
     class Model(BaseModel):
         value: RootModel[int]
 
     assert Model(value=42).value == RootModel[int](42)
 
 
+def test_root_model_base_model_equality():
+    class R(RootModel[int]):
+        pass
+
+    class B(BaseModel):
+        root: int
+
+    assert R(42) != B(root=42)
+    assert B(root=42) != R(42)
+
+
 @pytest.mark.xfail(reason='TODO: raise error for `extra` with `RootModel`')
 @pytest.mark.parametrize('extra_value', ['ignore', 'allow', 'forbid'])
 def test_extra_error(extra_value):
     with pytest.raises(PydanticUserError, match='extra'):
 
         class Model(RootModel[int]):
             model_config = ConfigDict(extra=extra_value)
```

### Comparing `pydantic-2.0b1/tests/test_serialize.py` & `pydantic-2.0b2/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_strict.py` & `pydantic-2.0b2/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_structural_pattern_matching.py` & `pydantic-2.0b2/tests/test_structural_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_tools.py` & `pydantic-2.0b2/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_type_adapter.py` & `pydantic-2.0b2/tests/test_type_adapter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import sys
+from dataclasses import dataclass
 from typing import Any, Dict, ForwardRef, Generic, List, NamedTuple, Tuple, TypeVar, Union
 
 import pytest
 from pydantic_core import ValidationError
 from typing_extensions import TypeAlias, TypedDict
 
 from pydantic import BaseModel, TypeAdapter, ValidationInfo, field_validator
@@ -190,7 +191,60 @@
             return v
 
     validator = TypeAdapter(Model)
     validator.validate_json(json.dumps({'x': 1}))
     validator.validate_json(json.dumps({'x': 1}), context=None)
     validator.validate_json(json.dumps({'x': 1}), context={'foo': 'bar'})
     assert contexts == []
+
+
+def test_validate_python_from_attributes() -> None:
+    class Model(BaseModel):
+        x: int
+
+    class ModelFromAttributesTrue(Model):
+        model_config = ConfigDict(from_attributes=True)
+
+    class ModelFromAttributesFalse(Model):
+        model_config = ConfigDict(from_attributes=False)
+
+    @dataclass
+    class UnrelatedClass:
+        x: int = 1
+
+    input = UnrelatedClass(1)
+
+    ta = TypeAdapter(Model)
+
+    for from_attributes in (False, None):
+        with pytest.raises(ValidationError) as exc_info:
+            ta.validate_python(UnrelatedClass(), from_attributes=from_attributes)
+        assert exc_info.value.errors(include_url=False) == [
+            {'type': 'dict_type', 'loc': (), 'msg': 'Input should be a valid dictionary', 'input': input}
+        ]
+
+    res = ta.validate_python(UnrelatedClass(), from_attributes=True)
+    assert res == Model(x=1)
+
+    ta = TypeAdapter(ModelFromAttributesTrue)
+
+    with pytest.raises(ValidationError) as exc_info:
+        ta.validate_python(UnrelatedClass(), from_attributes=False)
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'dict_type', 'loc': (), 'msg': 'Input should be a valid dictionary', 'input': input}
+    ]
+
+    for from_attributes in (True, None):
+        res = ta.validate_python(UnrelatedClass(), from_attributes=from_attributes)
+        assert res == ModelFromAttributesTrue(x=1)
+
+    ta = TypeAdapter(ModelFromAttributesFalse)
+
+    for from_attributes in (False, None):
+        with pytest.raises(ValidationError) as exc_info:
+            ta.validate_python(UnrelatedClass(), from_attributes=from_attributes)
+        assert exc_info.value.errors(include_url=False) == [
+            {'type': 'dict_type', 'loc': (), 'msg': 'Input should be a valid dictionary', 'input': input}
+        ]
+
+    res = ta.validate_python(UnrelatedClass(), from_attributes=True)
+    assert res == ModelFromAttributesFalse(x=1)
```

### Comparing `pydantic-2.0b1/tests/test_type_alias_type.py` & `pydantic-2.0b2/tests/test_type_alias_type.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_types.py` & `pydantic-2.0b2/tests/test_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -3744,20 +3744,30 @@
     assert not f.pattern.match(non_matching_value)
 
     # Check that pre-compiled patterns are accepted unchanged
     p = re.compile(pattern_value)
     f2 = Foobar(pattern=p)
     assert f2.pattern is p
 
-    # assert Foobar.model_json_schema() == {
-    #     'type': 'object',
-    #     'title': 'Foobar',
-    #     'properties': {'pattern': {'type': 'string', 'format': 'regex', 'title': 'Pattern'}},
-    #     'required': ['pattern'],
-    # }
+    assert Foobar.model_json_schema() == {
+        'type': 'object',
+        'title': 'Foobar',
+        'properties': {'pattern': {'type': 'string', 'format': 'regex', 'title': 'Pattern'}},
+        'required': ['pattern'],
+    }
+
+
+def test_pattern_with_invalid_param():
+    with pytest.raises(
+        PydanticSchemaGenerationError,
+        match=re.escape('Unable to generate pydantic-core schema for typing.Pattern[int].'),
+    ):
+
+        class Foo(BaseModel):
+            pattern: Pattern[int]
 
 
 @pytest.mark.parametrize(
     ('pattern_type', 'pattern_value', 'error_type', 'error_msg'),
     [
         pytest.param(
             re.Pattern,
```

### Comparing `pydantic-2.0b1/tests/test_types_namedtuple.py` & `pydantic-2.0b2/tests/test_types_namedtuple.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_types_payment_card_number.py` & `pydantic-2.0b2/tests/test_types_payment_card_number.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_types_typeddict.py` & `pydantic-2.0b2/tests/test_types_typeddict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_typing.py` & `pydantic-2.0b2/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_utils.py` & `pydantic-2.0b2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_v1.py` & `pydantic-2.0b2/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_validate_call.py` & `pydantic-2.0b2/tests/test_validate_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -548,14 +548,22 @@
 
     assert foo(b=10, d=1) == 11
     assert foo(a=10, d=1) == 11
     assert foo(b=10, c=1) == 11
     assert foo(a=10, c=1) == 11
 
 
+def test_validate_return():
+    @validate_call(config=dict(validate_return=True))
+    def foo(a: int, b: int) -> int:
+        return a + b
+
+    assert foo(1, 2) == 3
+
+
 def test_validate_all():
     @validate_call(config=dict(validate_default=True))
     def foo(dt: datetime = Field(default_factory=lambda: 946684800)):
         return dt
 
     assert foo() == datetime(2000, 1, 1)
     assert foo(0) == datetime(1970, 1, 1)
```

### Comparing `pydantic-2.0b1/tests/test_validators.py` & `pydantic-2.0b2/tests/test_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1008,14 +1008,29 @@
             @classmethod
             def check_foobar(cls, v: Any):
                 return v + 1
 
     assert Model(foobar={1: 1}).foobar == {1: 2}
 
 
+def test_validation_each_item_invalid_type():
+    with pytest.raises(
+        TypeError, match=re.escape('@validator(..., each_item=True)` cannot be applied to fields with a schema of int')
+    ):
+        with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
+
+            class Model(BaseModel):
+                foobar: int
+
+                @validator('foobar', each_item=True)
+                @classmethod
+                def check_foobar(cls, v: Any):
+                    ...
+
+
 def test_validation_each_item_nullable():
     with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
 
         class Model(BaseModel):
             foobar: Optional[List[int]]
 
             @validator('foobar', each_item=True)
```

### Comparing `pydantic-2.0b1/tests/test_validators_dataclass.py` & `pydantic-2.0b2/tests/test_validators_dataclass.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/test_version.py` & `pydantic-2.0b2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/test_mypy.py` & `pydantic-2.0b2/tests/mypy/test_mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/configs/mypy-plugin-strict-no-any.ini` & `pydantic-2.0b2/tests/mypy/configs/mypy-plugin-strict-no-any.ini`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/configs/pyproject-default.toml` & `pydantic-2.0b2/tests/mypy/configs/pyproject-default.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/configs/pyproject-plugin-bad-param.toml` & `pydantic-2.0b2/tests/mypy/configs/pyproject-plugin-bad-param.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/configs/pyproject-plugin-strict.toml` & `pydantic-2.0b2/tests/mypy/configs/pyproject-plugin-strict.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/configs/pyproject-plugin.toml` & `pydantic-2.0b2/tests/mypy/configs/pyproject-plugin.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/modules/computed_fields.py` & `pydantic-2.0b2/tests/mypy/modules/computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/modules/fail4.py` & `pydantic-2.0b2/tests/mypy/modules/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/modules/plugin_default_factory.py` & `pydantic-2.0b2/tests/mypy/modules/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/modules/plugin_fail.py` & `pydantic-2.0b2/tests/mypy/modules/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/modules/plugin_fail_baseConfig.py` & `pydantic-2.0b2/tests/mypy/modules/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/modules/plugin_success.py` & `pydantic-2.0b2/tests/mypy/modules/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/modules/plugin_success_baseConfig.py` & `pydantic-2.0b2/tests/mypy/modules/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/modules/success.py` & `pydantic-2.0b2/tests/mypy/modules/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/outputs/latest/fail4.txt` & `pydantic-2.0b2/tests/mypy/outputs/latest/fail4.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt` & `pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt` & `pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-strict.txt` & `pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail-strict.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail.txt` & `pydantic-2.0b2/tests/mypy/outputs/latest/plugin-fail.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/tests/pyright/pyright_example.py` & `pydantic-2.0b2/tests/pyright/pyright_example.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/.gitignore` & `pydantic-2.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/LICENSE` & `pydantic-2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/pyproject.toml` & `pydantic-2.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0b1/PKG-INFO` & `pydantic-2.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic
-Version: 2.0b1
+Version: 2.0b2
 Summary: Data validation using Python type hints
 Project-URL: Homepage, https://github.com/pydantic/pydantic
 Project-URL: Documentation, https://docs.pydantic.dev
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic
 Project-URL: Changelog, https://docs.pydantic.dev/changelog
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Terrence Dorsey <terry@pydantic.dev>, David Montague <david@pydantic.dev>
@@ -108,14 +108,20 @@
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/pydantic/security/policy).
 
 ## Changelog
 
+## v2.0b2 (2023-06-03)
+
+Add `from_attributes` runtime flag to `TypeAdapter.validate_python` and `BaseModel.model_validate`.
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b2)
+
 ## v2.0b1 (2023-06-01)
 
 First beta pre-release of Pydantic V2
 
 See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b1)
 
 ## v2.0a4 (2023-05-05)
```

