# Comparing `tmp/woke-3.3.0.tar.gz` & `tmp/woke-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woke-3.3.0.tar", max compression
+gzip compressed data, was "woke-3.4.0.tar", max compression
```

## Comparing `woke-3.3.0.tar` & `woke-3.4.0.tar`

### file list

```diff
@@ -1,238 +1,240 @@
--rw-r--r--   0        0        0      751 2023-04-24 12:08:38.351342 woke-3.3.0/LICENSE
--rw-r--r--   0        0        0     3423 2023-04-24 12:08:38.358009 woke-3.3.0/README.md
--rw-r--r--   0        0        0     2655 2023-04-24 12:09:29.024419 woke-3.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.388009 woke-3.3.0/woke/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/__init__.py
--rw-r--r--   0        0        0    20349 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/cfg.py
--rw-r--r--   0        0        0     1013 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/__init__.py
--rw-r--r--   0        0        0    21690 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/api.py
--rw-r--r--   0        0        0       61 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/axelar/__init__.py
--rw-r--r--   0        0        0    14739 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/axelar/proxy_contract_id.py
--rw-r--r--   0        0        0     6292 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/balance_state_var.py
--rw-r--r--   0        0        0     4759 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/bug_empty_byte_array_copy.py
--rw-r--r--   0        0        0     1777 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/call_options_not_called.py
--rw-r--r--   0        0        0     4162 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/missing_return.py
--rw-r--r--   0        0        0     3013 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/msg_value_nonpayable_function.py
--rw-r--r--   0        0        0     8578 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
--rw-r--r--   0        0        0    17003 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/ownable.py
--rw-r--r--   0        0        0    23312 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/proxy_contract_selector_clashes.py
--rw-r--r--   0        0        0    13896 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/reentrancy.py
--rw-r--r--   0        0        0     2766 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/unchecked_return_value.py
--rw-r--r--   0        0        0     6242 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/unsafe_delegatecall.py
--rw-r--r--   0        0        0     1344 2023-04-24 12:08:38.388009 woke-3.3.0/woke/analysis/detectors/unsafe_selfdestruct.py
--rw-r--r--   0        0        0     5982 2023-04-24 12:08:38.391342 woke-3.3.0/woke/analysis/detectors/unsafe_tx_origin.py
--rw-r--r--   0        0        0     1397 2023-04-24 12:08:38.391342 woke-3.3.0/woke/analysis/detectors/unused_contract.py
--rw-r--r--   0        0        0    12233 2023-04-24 12:08:38.391342 woke-3.3.0/woke/analysis/detectors/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/__init__.py
--rw-r--r--   0        0        0    10921 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/enums.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/__init__.py
--rw-r--r--   0        0        0     5939 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/abc.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/__init__.py
--rw-r--r--   0        0        0     5854 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/abc.py
--rw-r--r--   0        0        0    16242 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/contract_definition.py
--rw-r--r--   0        0        0     2460 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/enum_definition.py
--rw-r--r--   0        0        0     1360 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/enum_value.py
--rw-r--r--   0        0        0     4391 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/error_definition.py
--rw-r--r--   0        0        0     5162 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/event_definition.py
--rw-r--r--   0        0        0    18673 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/function_definition.py
--rw-r--r--   0        0        0    12886 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/modifier_definition.py
--rw-r--r--   0        0        0     2769 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/struct_definition.py
--rw-r--r--   0        0        0     2654 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/user_defined_value_type_definition.py
--rw-r--r--   0        0        0    17582 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/declaration/variable_declaration.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/__init__.py
--rw-r--r--   0        0        0     6583 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/abc.py
--rw-r--r--   0        0        0     3975 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/assignment.py
--rw-r--r--   0        0        0     2959 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/binary_operation.py
--rw-r--r--   0        0        0     2087 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/conditional.py
--rw-r--r--   0        0        0     1361 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/elementary_type_name_expression.py
--rw-r--r--   0        0        0     8923 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/function_call.py
--rw-r--r--   0        0        0     2132 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/function_call_options.py
--rw-r--r--   0        0        0     4446 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/identifier.py
--rw-r--r--   0        0        0     1996 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/index_access.py
--rw-r--r--   0        0        0     2661 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/index_range_access.py
--rw-r--r--   0        0        0     1437 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/literal.py
--rw-r--r--   0        0        0    18452 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/member_access.py
--rw-r--r--   0        0        0     1376 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/new_expression.py
--rw-r--r--   0        0        0     2186 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/tuple_expression.py
--rw-r--r--   0        0        0     3071 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/expression/unary_operation.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/__init__.py
--rw-r--r--   0        0        0     9095 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/identifier_path.py
--rw-r--r--   0        0        0     8845 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/import_directive.py
--rw-r--r--   0        0        0     3751 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/inheritance_specifier.py
--rw-r--r--   0        0        0     5699 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/modifier_invocation.py
--rw-r--r--   0        0        0     3456 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/override_specifier.py
--rw-r--r--   0        0        0     4305 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/parameter_list.py
--rw-r--r--   0        0        0     1529 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/pragma_directive.py
--rw-r--r--   0        0        0     9257 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/source_unit.py
--rw-r--r--   0        0        0     2314 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/structured_documentation.py
--rw-r--r--   0        0        0     4541 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/try_catch_clause.py
--rw-r--r--   0        0        0     5698 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/meta/using_for_directive.py
--rw-r--r--   0        0        0     4812 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/reference_resolver.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/__init__.py
--rw-r--r--   0        0        0     5607 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/abc.py
--rw-r--r--   0        0        0     3130 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/block.py
--rw-r--r--   0        0        0     1610 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/break_statement.py
--rw-r--r--   0        0        0     1634 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/continue_statement.py
--rw-r--r--   0        0        0     2563 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/do_while_statement.py
--rw-r--r--   0        0        0     2452 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/emit_statement.py
--rw-r--r--   0        0        0     6016 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/expression_statement.py
--rw-r--r--   0        0        0     5735 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/for_statement.py
--rw-r--r--   0        0        0     3423 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/if_statement.py
--rw-r--r--   0        0        0    10271 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/inline_assembly.py
--rw-r--r--   0        0        0     1582 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/placeholder_statement.py
--rw-r--r--   0        0        0     3336 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/return_statement.py
--rw-r--r--   0        0        0     2608 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/revert_statement.py
--rw-r--r--   0        0        0     3129 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/try_statement.py
--rw-r--r--   0        0        0     2449 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/unchecked_block.py
--rw-r--r--   0        0        0     4325 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/variable_declaration_statement.py
--rw-r--r--   0        0        0     2596 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/statement/while_statement.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/__init__.py
--rw-r--r--   0        0        0     4932 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/abc.py
--rw-r--r--   0        0        0     4036 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/array_type_name.py
--rw-r--r--   0        0        0     5647 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/elementary_type_name.py
--rw-r--r--   0        0        0     3971 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/function_type_name.py
--rw-r--r--   0        0        0     3922 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/mapping.py
--rw-r--r--   0        0        0     8333 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/type_name/user_defined_type_name.py
--rw-r--r--   0        0        0       36 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/utils/__init__.py
--rw-r--r--   0        0        0      589 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/utils/init_tuple.py
--rw-r--r--   0        0        0      578 2023-04-24 12:08:38.391342 woke-3.3.0/woke/ast/ir/yul/__init__.py
--rw-r--r--   0        0        0      703 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/abc.py
--rw-r--r--   0        0        0     1811 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/assignment.py
--rw-r--r--   0        0        0     4302 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/block.py
--rw-r--r--   0        0        0      300 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/break_statement.py
--rw-r--r--   0        0        0     1199 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/case_statement.py
--rw-r--r--   0        0        0      303 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/continue_statement.py
--rw-r--r--   0        0        0     1658 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/expression_statement.py
--rw-r--r--   0        0        0     1893 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/for_loop.py
--rw-r--r--   0        0        0     2317 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/function_call.py
--rw-r--r--   0        0        0     2288 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/function_definition.py
--rw-r--r--   0        0        0     1492 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/identifier.py
--rw-r--r--   0        0        0     1582 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/if_statement.py
--rw-r--r--   0        0        0      300 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/leave.py
--rw-r--r--   0        0        0     1780 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/literal.py
--rw-r--r--   0        0        0     1796 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/switch.py
--rw-r--r--   0        0        0      920 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/typed_name.py
--rw-r--r--   0        0        0     2091 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/ir/yul/variable_declaration.py
--rw-r--r--   0        0        0    37545 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/nodes.py
--rw-r--r--   0        0        0    47040 2023-04-24 12:08:38.394675 woke-3.3.0/woke/ast/types.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/__init__.py
--rw-r--r--   0        0        0     3500 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/__main__.py
--rw-r--r--   0        0        0     7942 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/accounts.py
--rw-r--r--   0        0        0     4650 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/compile.py
--rw-r--r--   0        0        0       54 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/console.py
--rw-r--r--   0        0        0     3838 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/detect.py
--rw-r--r--   0        0        0     3791 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/fuzz.py
--rw-r--r--   0        0        0    11813 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/init.py
--rw-r--r--   0        0        0     1081 2023-04-24 12:08:38.394675 woke-3.3.0/woke/cli/lsp.py
--rw-r--r--   0        0        0     3154 2023-04-24 12:08:38.398009 woke-3.3.0/woke/cli/run.py
--rw-r--r--   0        0        0     4922 2023-04-24 12:08:38.398009 woke-3.3.0/woke/cli/svm.py
--rw-r--r--   0        0        0     2258 2023-04-24 12:08:38.398009 woke-3.3.0/woke/cli/test.py
--rw-r--r--   0        0        0      187 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/__init__.py
--rw-r--r--   0        0        0     1814 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/build_data_model.py
--rw-r--r--   0        0        0     3078 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/compilation_unit.py
--rw-r--r--   0        0        0    41519 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/compiler.py
--rw-r--r--   0        0        0       97 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/exceptions.py
--rw-r--r--   0        0        0      103 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/__init__.py
--rw-r--r--   0        0        0       48 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/exceptions.py
--rw-r--r--   0        0        0     8554 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/input_data_model.py
--rw-r--r--   0        0        0     8728 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/output_data_model.py
--rw-r--r--   0        0        0     3571 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/solc_frontend/solc_runner.py
--rw-r--r--   0        0        0     2455 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/source_path_resolver.py
--rw-r--r--   0        0        0     4819 2023-04-24 12:08:38.398009 woke-3.3.0/woke/compiler/source_unit_name_resolver.py
--rw-r--r--   0        0        0     1118 2023-04-24 12:08:38.398009 woke-3.3.0/woke/config/__init__.py
--rw-r--r--   0        0        0     6866 2023-04-24 12:08:38.398009 woke-3.3.0/woke/config/data_model.py
--rw-r--r--   0        0        0    12617 2023-04-24 12:08:38.398009 woke-3.3.0/woke/config/woke_config.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.3.0/woke/contracts/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.3.0/woke/contracts/woke/__init__.py
--rw-r--r--   0        0        0    64087 2023-04-24 12:08:38.398009 woke-3.3.0/woke/contracts/woke/console.sol
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.3.0/woke/core/__init__.py
--rw-r--r--   0        0        0      360 2023-04-24 12:08:38.398009 woke-3.3.0/woke/core/enums.py
--rw-r--r--   0        0        0    24824 2023-04-24 12:08:38.398009 woke-3.3.0/woke/core/solidity_version.py
--rw-r--r--   0        0        0      663 2023-04-24 12:08:38.398009 woke-3.3.0/woke/deployment/__init__.py
--rw-r--r--   0        0        0    14901 2023-04-24 12:08:38.398009 woke-3.3.0/woke/deployment/core.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/__init__.py
--rw-r--r--   0        0        0     4552 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/blocks.py
--rw-r--r--   0        0        0    28998 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/call_trace.py
--rw-r--r--   0        0        0    25863 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/chain_interfaces.py
--rw-r--r--   0        0        0     1132 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/constants.py
--rw-r--r--   0        0        0    95503 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/core.py
--rw-r--r--   0        0        0     7270 2023-04-24 12:08:38.398009 woke-3.3.0/woke/development/globals.py
--rw-r--r--   0        0        0   161115 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/hardhat_console.py
--rw-r--r--   0        0        0     1093 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/internal.py
--rw-r--r--   0        0        0       39 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/__init__.py
--rw-r--r--   0        0        0      302 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/abc.py
--rw-r--r--   0        0        0     2070 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/communicator.py
--rw-r--r--   0        0        0      821 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/http.py
--rw-r--r--   0        0        0     2733 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/ipc.py
--rw-r--r--   0        0        0      625 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/json_rpc/websocket.py
--rw-r--r--   0        0        0     6572 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/primitive_types.py
--rw-r--r--   0        0        0    88054 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/pytypes_generator.py
--rw-r--r--   0        0        0    26697 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/transactions.py
--rw-r--r--   0        0        0     7389 2023-04-24 12:08:38.401342 woke-3.3.0/woke/development/utils.py
--rw-r--r--   0        0        0       47 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/__init__.py
--rw-r--r--   0        0        0      310 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/__init__.py
--rw-r--r--   0        0        0     3648 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/generate_control_flow_graph.py
--rw-r--r--   0        0        0      938 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/generate_imports_graph.py
--rw-r--r--   0        0        0     4247 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/generate_inheritance_graph.py
--rw-r--r--   0        0        0     2163 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/commands/generate_linearized_inheritance_graph.py
--rw-r--r--   0        0        0    31330 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/common_structures.py
--rw-r--r--   0        0        0     1721 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/context.py
--rw-r--r--   0        0        0     2574 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/document_sync.py
--rw-r--r--   0        0        0      130 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/enums.py
--rw-r--r--   0        0        0      471 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/__init__.py
--rw-r--r--   0        0        0     9946 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/code_lens.py
--rw-r--r--   0        0        0    14531 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/completion.py
--rw-r--r--   0        0        0     9948 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/definition.py
--rw-r--r--   0        0        0     1446 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/diagnostic.py
--rw-r--r--   0        0        0     3908 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/document_link.py
--rw-r--r--   0        0        0     8407 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/document_symbol.py
--rw-r--r--   0        0        0    11205 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/hover.py
--rw-r--r--   0        0        0     3850 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/implementation.py
--rw-r--r--   0        0        0     5092 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/references.py
--rw-r--r--   0        0        0     8935 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/rename.py
--rw-r--r--   0        0        0     9505 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/type_definition.py
--rw-r--r--   0        0        0    11043 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/features/type_hierarchy.py
--rw-r--r--   0        0        0    37512 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/lsp_compiler.py
--rw-r--r--   0        0        0      328 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/lsp_data_model.py
--rw-r--r--   0        0        0     5551 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/methods.py
--rw-r--r--   0        0        0     1897 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/protocol_structures.py
--rw-r--r--   0        0        0     2229 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/rpc_protocol.py
--rw-r--r--   0        0        0    36478 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/server.py
--rw-r--r--   0        0        0     6541 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/server_capabilities.py
--rw-r--r--   0        0        0       86 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/utils/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/utils/position.py
--rw-r--r--   0        0        0      459 2023-04-24 12:08:38.401342 woke-3.3.0/woke/lsp/utils/uri.py
--rw-r--r--   0        0        0       50 2023-04-24 12:08:38.401342 woke-3.3.0/woke/regex_parser/__init__.py
--rw-r--r--   0        0        0     1690 2023-04-24 12:08:38.401342 woke-3.3.0/woke/regex_parser/solidity_import.py
--rw-r--r--   0        0        0     6653 2023-04-24 12:08:38.401342 woke-3.3.0/woke/regex_parser/solidity_parser.py
--rw-r--r--   0        0        0       36 2023-04-24 12:08:38.401342 woke-3.3.0/woke/svm/__init__.py
--rw-r--r--   0        0        0     1810 2023-04-24 12:08:38.404675 woke-3.3.0/woke/svm/abc.py
--rw-r--r--   0        0        0      270 2023-04-24 12:08:38.404675 woke-3.3.0/woke/svm/exceptions.py
--rw-r--r--   0        0        0    11716 2023-04-24 12:08:38.404675 woke-3.3.0/woke/svm/svm.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.404675 woke-3.3.0/woke/templates/scripts/__init__.py
--rw-r--r--   0        0        0      184 2023-04-24 12:08:38.404675 woke-3.3.0/woke/templates/scripts/deploy.py
--rw-r--r--   0        0        0        0 2023-04-24 12:08:38.404675 woke-3.3.0/woke/templates/tests/__init__.py
--rw-r--r--   0        0        0      140 2023-04-24 12:08:38.404675 woke-3.3.0/woke/templates/tests/test_default.py
--rw-r--r--   0        0        0      663 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/__init__.py
--rw-r--r--   0        0        0    10878 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/core.py
--rw-r--r--   0        0        0    24360 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/coverage.py
--rw-r--r--   0        0        0      187 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/fuzzing/__init__.py
--rw-r--r--   0        0        0     4999 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/fuzzing/fuzz_test.py
--rw-r--r--   0        0        0    10795 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/fuzzing/fuzzer.py
--rw-r--r--   0        0        0     5780 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/fuzzing/generators.py
--rw-r--r--   0        0        0      298 2023-04-24 12:08:38.404675 woke-3.3.0/woke/testing/pytest_plugin.py
--rw-r--r--   0        0        0      170 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/__init__.py
--rw-r--r--   0        0        0      560 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/context_managers.py
--rw-r--r--   0        0        0      513 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/decorators.py
--rw-r--r--   0        0        0      158 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/enums.py
--rw-r--r--   0        0        0     1699 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/file_utils.py
--rw-r--r--   0        0        0      383 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/keyed_default_dict.py
--rw-r--r--   0        0        0      194 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/networking.py
--rw-r--r--   0        0        0     1017 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/openzeppelin.py
--rw-r--r--   0        0        0      630 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/string.py
--rw-r--r--   0        0        0     1742 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/tee.py
--rw-r--r--   0        0        0     3765 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/threaded_child_watcher.py
--rw-r--r--   0        0        0      423 2023-04-24 12:08:38.404675 woke-3.3.0/woke/utils/version.py
--rw-r--r--   0        0        0     6058 1970-01-01 00:00:00.000000 woke-3.3.0/setup.py
--rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 woke-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0      751 2023-04-24 12:08:38.351342 woke-3.4.0/LICENSE
+-rw-r--r--   0        0        0     3415 2023-05-12 13:33:59.511209 woke-3.4.0/README.md
+-rw-r--r--   0        0        0     2720 2023-05-12 13:34:18.427778 woke-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.388009 woke-3.4.0/woke/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/__init__.py
+-rw-r--r--   0        0        0    20473 2023-05-11 12:18:16.997856 woke-3.4.0/woke/analysis/cfg.py
+-rw-r--r--   0        0        0     1013 2023-05-10 19:31:50.999588 woke-3.4.0/woke/analysis/detectors/__init__.py
+-rw-r--r--   0        0        0    21743 2023-05-11 12:18:16.997856 woke-3.4.0/woke/analysis/detectors/api.py
+-rw-r--r--   0        0        0       61 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/detectors/axelar/__init__.py
+-rw-r--r--   0        0        0    15183 2023-05-11 12:18:16.997856 woke-3.4.0/woke/analysis/detectors/axelar/proxy_contract_id.py
+-rw-r--r--   0        0        0     6389 2023-05-11 12:18:16.997856 woke-3.4.0/woke/analysis/detectors/balance_state_var.py
+-rw-r--r--   0        0        0     4759 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/detectors/bug_empty_byte_array_copy.py
+-rw-r--r--   0        0        0     1777 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/detectors/call_options_not_called.py
+-rw-r--r--   0        0        0     4162 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/detectors/missing_return.py
+-rw-r--r--   0        0        0     3013 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/detectors/msg_value_nonpayable_function.py
+-rw-r--r--   0        0        0     8723 2023-05-12 13:33:59.511209 woke-3.4.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
+-rw-r--r--   0        0        0    17299 2023-05-11 12:18:16.997856 woke-3.4.0/woke/analysis/detectors/ownable.py
+-rw-r--r--   0        0        0    23312 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/detectors/proxy_contract_selector_clashes.py
+-rw-r--r--   0        0        0    13982 2023-05-11 12:18:16.997856 woke-3.4.0/woke/analysis/detectors/reentrancy.py
+-rw-r--r--   0        0        0     2766 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/detectors/unchecked_return_value.py
+-rw-r--r--   0        0        0     6242 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/detectors/unsafe_delegatecall.py
+-rw-r--r--   0        0        0     1344 2023-04-24 12:08:38.388009 woke-3.4.0/woke/analysis/detectors/unsafe_selfdestruct.py
+-rw-r--r--   0        0        0     5982 2023-04-24 12:08:38.391342 woke-3.4.0/woke/analysis/detectors/unsafe_tx_origin.py
+-rw-r--r--   0        0        0     1397 2023-04-24 12:08:38.391342 woke-3.4.0/woke/analysis/detectors/unused_contract.py
+-rw-r--r--   0        0        0    12233 2023-05-10 19:31:56.089565 woke-3.4.0/woke/analysis/detectors/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/__init__.py
+-rw-r--r--   0        0        0    10947 2023-05-12 13:33:59.511209 woke-3.4.0/woke/ast/enums.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/__init__.py
+-rw-r--r--   0        0        0     5941 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/abc.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/declaration/__init__.py
+-rw-r--r--   0        0        0     5854 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/declaration/abc.py
+-rw-r--r--   0        0        0    16974 2023-05-12 13:33:59.511209 woke-3.4.0/woke/ast/ir/declaration/contract_definition.py
+-rw-r--r--   0        0        0     3079 2023-05-12 13:33:59.511209 woke-3.4.0/woke/ast/ir/declaration/enum_definition.py
+-rw-r--r--   0        0        0     1361 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/declaration/enum_value.py
+-rw-r--r--   0        0        0     4408 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/declaration/error_definition.py
+-rw-r--r--   0        0        0     5162 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/declaration/event_definition.py
+-rw-r--r--   0        0        0    18683 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/declaration/function_definition.py
+-rw-r--r--   0        0        0    12891 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/declaration/modifier_definition.py
+-rw-r--r--   0        0        0     3414 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/declaration/struct_definition.py
+-rw-r--r--   0        0        0     2654 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/declaration/user_defined_value_type_definition.py
+-rw-r--r--   0        0        0    19473 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/declaration/variable_declaration.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/__init__.py
+-rw-r--r--   0        0        0     6583 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/abc.py
+-rw-r--r--   0        0        0     4063 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/expression/assignment.py
+-rw-r--r--   0        0        0     2959 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/binary_operation.py
+-rw-r--r--   0        0        0     2087 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/conditional.py
+-rw-r--r--   0        0        0     1361 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/elementary_type_name_expression.py
+-rw-r--r--   0        0        0     8933 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/expression/function_call.py
+-rw-r--r--   0        0        0     2142 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/expression/function_call_options.py
+-rw-r--r--   0        0        0     5709 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/expression/identifier.py
+-rw-r--r--   0        0        0     1996 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/index_access.py
+-rw-r--r--   0        0        0     2661 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/index_range_access.py
+-rw-r--r--   0        0        0     1437 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/literal.py
+-rw-r--r--   0        0        0    19431 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/expression/member_access.py
+-rw-r--r--   0        0        0     1376 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/new_expression.py
+-rw-r--r--   0        0        0     2191 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/expression/tuple_expression.py
+-rw-r--r--   0        0        0     3071 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/expression/unary_operation.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/meta/__init__.py
+-rw-r--r--   0        0        0    10965 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/meta/identifier_path.py
+-rw-r--r--   0        0        0     8998 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/meta/import_directive.py
+-rw-r--r--   0        0        0     3752 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/meta/inheritance_specifier.py
+-rw-r--r--   0        0        0     5700 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/meta/modifier_invocation.py
+-rw-r--r--   0        0        0     3462 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/meta/override_specifier.py
+-rw-r--r--   0        0        0     4311 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/meta/parameter_list.py
+-rw-r--r--   0        0        0     1534 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/meta/pragma_directive.py
+-rw-r--r--   0        0        0     9307 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/meta/source_unit.py
+-rw-r--r--   0        0        0     2315 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/meta/structured_documentation.py
+-rw-r--r--   0        0        0     4541 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/meta/try_catch_clause.py
+-rw-r--r--   0        0        0     5698 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/meta/using_for_directive.py
+-rw-r--r--   0        0        0     4812 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/reference_resolver.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/statement/__init__.py
+-rw-r--r--   0        0        0     5608 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/statement/abc.py
+-rw-r--r--   0        0        0     3135 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/statement/block.py
+-rw-r--r--   0        0        0     1611 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/statement/break_statement.py
+-rw-r--r--   0        0        0     1635 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/statement/continue_statement.py
+-rw-r--r--   0        0        0     2563 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/statement/do_while_statement.py
+-rw-r--r--   0        0        0     2452 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/statement/emit_statement.py
+-rw-r--r--   0        0        0     6016 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/statement/expression_statement.py
+-rw-r--r--   0        0        0     5735 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/statement/for_statement.py
+-rw-r--r--   0        0        0     3423 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/statement/if_statement.py
+-rw-r--r--   0        0        0    10276 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/statement/inline_assembly.py
+-rw-r--r--   0        0        0     1583 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/statement/placeholder_statement.py
+-rw-r--r--   0        0        0     3336 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/statement/return_statement.py
+-rw-r--r--   0        0        0     2608 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/statement/revert_statement.py
+-rw-r--r--   0        0        0     3134 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/statement/try_statement.py
+-rw-r--r--   0        0        0     2454 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/statement/unchecked_block.py
+-rw-r--r--   0        0        0     4330 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/statement/variable_declaration_statement.py
+-rw-r--r--   0        0        0     2596 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/statement/while_statement.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/type_name/__init__.py
+-rw-r--r--   0        0        0     4932 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/type_name/abc.py
+-rw-r--r--   0        0        0     4092 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/type_name/array_type_name.py
+-rw-r--r--   0        0        0     5967 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/type_name/elementary_type_name.py
+-rw-r--r--   0        0        0     3987 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/type_name/function_type_name.py
+-rw-r--r--   0        0        0     3938 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/type_name/mapping.py
+-rw-r--r--   0        0        0    11314 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/type_name/user_defined_type_name.py
+-rw-r--r--   0        0        0       36 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/utils/__init__.py
+-rw-r--r--   0        0        0      589 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/utils/init_tuple.py
+-rw-r--r--   0        0        0      578 2023-04-24 12:08:38.391342 woke-3.4.0/woke/ast/ir/yul/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/yul/abc.py
+-rw-r--r--   0        0        0     1817 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/yul/assignment.py
+-rw-r--r--   0        0        0     4317 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/yul/block.py
+-rw-r--r--   0        0        0      301 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/yul/break_statement.py
+-rw-r--r--   0        0        0     1200 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/yul/case_statement.py
+-rw-r--r--   0        0        0      304 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/yul/continue_statement.py
+-rw-r--r--   0        0        0     1659 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/yul/expression_statement.py
+-rw-r--r--   0        0        0     1893 2023-04-24 12:08:38.394675 woke-3.4.0/woke/ast/ir/yul/for_loop.py
+-rw-r--r--   0        0        0     2323 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/yul/function_call.py
+-rw-r--r--   0        0        0     2298 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/yul/function_definition.py
+-rw-r--r--   0        0        0     1492 2023-04-24 12:08:38.394675 woke-3.4.0/woke/ast/ir/yul/identifier.py
+-rw-r--r--   0        0        0     1582 2023-04-24 12:08:38.394675 woke-3.4.0/woke/ast/ir/yul/if_statement.py
+-rw-r--r--   0        0        0      301 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/yul/leave.py
+-rw-r--r--   0        0        0     1781 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/yul/literal.py
+-rw-r--r--   0        0        0     1802 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/yul/switch.py
+-rw-r--r--   0        0        0      921 2023-05-11 12:18:16.997856 woke-3.4.0/woke/ast/ir/yul/typed_name.py
+-rw-r--r--   0        0        0     2097 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/ir/yul/variable_declaration.py
+-rw-r--r--   0        0        0    37866 2023-05-12 13:33:59.514542 woke-3.4.0/woke/ast/nodes.py
+-rw-r--r--   0        0        0    47087 2023-05-11 12:18:17.001189 woke-3.4.0/woke/ast/types.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.394675 woke-3.4.0/woke/cli/__init__.py
+-rw-r--r--   0        0        0     3501 2023-05-11 12:18:17.001189 woke-3.4.0/woke/cli/__main__.py
+-rw-r--r--   0        0        0     7942 2023-04-24 12:08:38.394675 woke-3.4.0/woke/cli/accounts.py
+-rw-r--r--   0        0        0     4650 2023-04-25 07:40:18.902645 woke-3.4.0/woke/cli/compile.py
+-rw-r--r--   0        0        0       54 2023-04-24 12:08:38.394675 woke-3.4.0/woke/cli/console.py
+-rw-r--r--   0        0        0     3838 2023-05-10 19:31:50.999588 woke-3.4.0/woke/cli/detect.py
+-rw-r--r--   0        0        0     3791 2023-04-24 12:08:38.394675 woke-3.4.0/woke/cli/fuzz.py
+-rw-r--r--   0        0        0    11813 2023-05-11 09:02:43.932954 woke-3.4.0/woke/cli/init.py
+-rw-r--r--   0        0        0     1081 2023-04-24 12:08:38.394675 woke-3.4.0/woke/cli/lsp.py
+-rw-r--r--   0        0        0     3154 2023-04-24 12:08:38.398009 woke-3.4.0/woke/cli/run.py
+-rw-r--r--   0        0        0     4922 2023-04-24 12:08:38.398009 woke-3.4.0/woke/cli/svm.py
+-rw-r--r--   0        0        0     2258 2023-05-10 19:31:50.999588 woke-3.4.0/woke/cli/test.py
+-rw-r--r--   0        0        0      187 2023-04-24 12:08:38.398009 woke-3.4.0/woke/compiler/__init__.py
+-rw-r--r--   0        0        0     1814 2023-04-24 12:08:38.398009 woke-3.4.0/woke/compiler/build_data_model.py
+-rw-r--r--   0        0        0     3120 2023-05-11 12:18:17.001189 woke-3.4.0/woke/compiler/compilation_unit.py
+-rw-r--r--   0        0        0    41479 2023-05-11 12:18:17.001189 woke-3.4.0/woke/compiler/compiler.py
+-rw-r--r--   0        0        0       97 2023-04-24 12:08:38.398009 woke-3.4.0/woke/compiler/exceptions.py
+-rw-r--r--   0        0        0      103 2023-04-24 12:08:38.398009 woke-3.4.0/woke/compiler/solc_frontend/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-24 12:08:38.398009 woke-3.4.0/woke/compiler/solc_frontend/exceptions.py
+-rw-r--r--   0        0        0     8554 2023-04-24 12:08:38.398009 woke-3.4.0/woke/compiler/solc_frontend/input_data_model.py
+-rw-r--r--   0        0        0     8728 2023-04-24 12:08:38.398009 woke-3.4.0/woke/compiler/solc_frontend/output_data_model.py
+-rw-r--r--   0        0        0     3571 2023-04-24 12:08:38.398009 woke-3.4.0/woke/compiler/solc_frontend/solc_runner.py
+-rw-r--r--   0        0        0     2455 2023-04-24 12:08:38.398009 woke-3.4.0/woke/compiler/source_path_resolver.py
+-rw-r--r--   0        0        0     4813 2023-05-11 12:18:17.001189 woke-3.4.0/woke/compiler/source_unit_name_resolver.py
+-rw-r--r--   0        0        0     1118 2023-04-24 12:08:38.398009 woke-3.4.0/woke/config/__init__.py
+-rw-r--r--   0        0        0     6912 2023-05-12 13:33:59.514542 woke-3.4.0/woke/config/data_model.py
+-rw-r--r--   0        0        0    12682 2023-05-12 13:33:59.514542 woke-3.4.0/woke/config/woke_config.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.4.0/woke/contracts/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.4.0/woke/contracts/woke/__init__.py
+-rw-r--r--   0        0        0    64087 2023-04-24 12:08:38.398009 woke-3.4.0/woke/contracts/woke/console.sol
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.4.0/woke/core/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-12 13:33:59.514542 woke-3.4.0/woke/core/enums.py
+-rw-r--r--   0        0        0    24829 2023-05-12 13:33:59.514542 woke-3.4.0/woke/core/solidity_version.py
+-rw-r--r--   0        0        0      678 2023-05-12 13:33:59.514542 woke-3.4.0/woke/deployment/__init__.py
+-rw-r--r--   0        0        0    14848 2023-05-11 12:18:17.001189 woke-3.4.0/woke/deployment/core.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.398009 woke-3.4.0/woke/development/__init__.py
+-rw-r--r--   0        0        0     4552 2023-04-24 12:08:38.398009 woke-3.4.0/woke/development/blocks.py
+-rw-r--r--   0        0        0    28963 2023-05-11 12:18:17.001189 woke-3.4.0/woke/development/call_trace.py
+-rw-r--r--   0        0        0    25863 2023-04-25 07:36:54.143450 woke-3.4.0/woke/development/chain_interfaces.py
+-rw-r--r--   0        0        0     1132 2023-04-24 12:08:38.398009 woke-3.4.0/woke/development/constants.py
+-rw-r--r--   0        0        0    96257 2023-05-12 13:33:59.514542 woke-3.4.0/woke/development/core.py
+-rw-r--r--   0        0        0     7270 2023-04-25 07:36:54.143450 woke-3.4.0/woke/development/globals.py
+-rw-r--r--   0        0        0   161115 2023-04-24 12:08:38.401342 woke-3.4.0/woke/development/hardhat_console.py
+-rw-r--r--   0        0        0     1093 2023-04-24 12:08:38.401342 woke-3.4.0/woke/development/internal.py
+-rw-r--r--   0        0        0       39 2023-04-24 12:08:38.401342 woke-3.4.0/woke/development/json_rpc/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-24 12:08:38.401342 woke-3.4.0/woke/development/json_rpc/abc.py
+-rw-r--r--   0        0        0     2070 2023-04-24 12:08:38.401342 woke-3.4.0/woke/development/json_rpc/communicator.py
+-rw-r--r--   0        0        0      821 2023-04-24 12:08:38.401342 woke-3.4.0/woke/development/json_rpc/http.py
+-rw-r--r--   0        0        0     2912 2023-05-11 12:18:17.001189 woke-3.4.0/woke/development/json_rpc/ipc.py
+-rw-r--r--   0        0        0      625 2023-04-24 12:08:38.401342 woke-3.4.0/woke/development/json_rpc/websocket.py
+-rw-r--r--   0        0        0     6572 2023-04-24 12:08:38.401342 woke-3.4.0/woke/development/primitive_types.py
+-rw-r--r--   0        0        0    90006 2023-05-12 13:33:59.514542 woke-3.4.0/woke/development/pytypes_generator.py
+-rw-r--r--   0        0        0    28061 2023-05-12 13:33:59.514542 woke-3.4.0/woke/development/transactions.py
+-rw-r--r--   0        0        0     7389 2023-04-29 08:18:37.950570 woke-3.4.0/woke/development/utils.py
+-rw-r--r--   0        0        0       47 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-10 19:31:50.999588 woke-3.4.0/woke/lsp/commands/__init__.py
+-rw-r--r--   0        0        0     4033 2023-05-11 12:18:17.001189 woke-3.4.0/woke/lsp/commands/generate_control_flow_graph.py
+-rw-r--r--   0        0        0     1097 2023-05-11 12:18:17.001189 woke-3.4.0/woke/lsp/commands/generate_imports_graph.py
+-rw-r--r--   0        0        0     4247 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/commands/generate_inheritance_graph.py
+-rw-r--r--   0        0        0     2163 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/commands/generate_linearized_inheritance_graph.py
+-rw-r--r--   0        0        0    31491 2023-05-11 12:18:17.001189 woke-3.4.0/woke/lsp/common_structures.py
+-rw-r--r--   0        0        0     1900 2023-05-11 12:18:17.001189 woke-3.4.0/woke/lsp/context.py
+-rw-r--r--   0        0        0     2574 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/document_sync.py
+-rw-r--r--   0        0        0      130 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/enums.py
+-rw-r--r--   0        0        0      471 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/features/__init__.py
+-rw-r--r--   0        0        0     6969 2023-05-12 13:33:59.514542 woke-3.4.0/woke/lsp/features/code_action.py
+-rw-r--r--   0        0        0    10904 2023-05-11 12:18:17.001189 woke-3.4.0/woke/lsp/features/code_lens.py
+-rw-r--r--   0        0        0    19824 2023-05-12 13:33:59.514542 woke-3.4.0/woke/lsp/features/completion.py
+-rw-r--r--   0        0        0     9948 2023-05-08 19:20:45.625567 woke-3.4.0/woke/lsp/features/definition.py
+-rw-r--r--   0        0        0     1446 2023-04-25 07:40:14.399401 woke-3.4.0/woke/lsp/features/diagnostic.py
+-rw-r--r--   0        0        0     4305 2023-05-12 13:33:59.514542 woke-3.4.0/woke/lsp/features/document_link.py
+-rw-r--r--   0        0        0     8407 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/features/document_symbol.py
+-rw-r--r--   0        0        0    17901 2023-05-11 12:18:17.001189 woke-3.4.0/woke/lsp/features/hover.py
+-rw-r--r--   0        0        0     3850 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/features/implementation.py
+-rw-r--r--   0        0        0     5092 2023-05-06 18:57:44.155992 woke-3.4.0/woke/lsp/features/references.py
+-rw-r--r--   0        0        0     8935 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/features/rename.py
+-rw-r--r--   0        0        0     9505 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/features/type_definition.py
+-rw-r--r--   0        0        0    11043 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/features/type_hierarchy.py
+-rw-r--r--   0        0        0    39251 2023-05-11 12:18:17.001189 woke-3.4.0/woke/lsp/lsp_compiler.py
+-rw-r--r--   0        0        0      328 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/lsp_data_model.py
+-rw-r--r--   0        0        0     8941 2023-05-12 13:33:59.514542 woke-3.4.0/woke/lsp/lsp_parser.py
+-rw-r--r--   0        0        0     5551 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/methods.py
+-rw-r--r--   0        0        0     1897 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/protocol_structures.py
+-rw-r--r--   0        0        0     2229 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/rpc_protocol.py
+-rw-r--r--   0        0        0    37738 2023-05-11 12:18:17.001189 woke-3.4.0/woke/lsp/server.py
+-rw-r--r--   0        0        0     6597 2023-05-11 12:18:17.001189 woke-3.4.0/woke/lsp/server_capabilities.py
+-rw-r--r--   0        0        0       86 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/utils/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/utils/position.py
+-rw-r--r--   0        0        0      459 2023-04-24 12:08:38.401342 woke-3.4.0/woke/lsp/utils/uri.py
+-rw-r--r--   0        0        0       50 2023-04-24 12:08:38.401342 woke-3.4.0/woke/regex_parser/__init__.py
+-rw-r--r--   0        0        0     1690 2023-04-24 12:08:38.401342 woke-3.4.0/woke/regex_parser/solidity_import.py
+-rw-r--r--   0        0        0     6653 2023-05-10 19:31:50.999588 woke-3.4.0/woke/regex_parser/solidity_parser.py
+-rw-r--r--   0        0        0       36 2023-04-24 12:08:38.401342 woke-3.4.0/woke/svm/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-12 13:33:59.514542 woke-3.4.0/woke/svm/abc.py
+-rw-r--r--   0        0        0      270 2023-04-24 12:08:38.404675 woke-3.4.0/woke/svm/exceptions.py
+-rw-r--r--   0        0        0    11721 2023-05-12 13:33:59.514542 woke-3.4.0/woke/svm/svm.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.404675 woke-3.4.0/woke/templates/scripts/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-24 12:08:38.404675 woke-3.4.0/woke/templates/scripts/deploy.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:08:38.404675 woke-3.4.0/woke/templates/tests/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-24 12:08:38.404675 woke-3.4.0/woke/templates/tests/test_default.py
+-rw-r--r--   0        0        0      678 2023-05-12 13:33:59.514542 woke-3.4.0/woke/testing/__init__.py
+-rw-r--r--   0        0        0    10878 2023-04-25 07:36:54.146783 woke-3.4.0/woke/testing/core.py
+-rw-r--r--   0        0        0    24381 2023-05-12 13:33:59.514542 woke-3.4.0/woke/testing/coverage.py
+-rw-r--r--   0        0        0      187 2023-04-24 12:08:38.404675 woke-3.4.0/woke/testing/fuzzing/__init__.py
+-rw-r--r--   0        0        0     4999 2023-04-24 12:08:38.404675 woke-3.4.0/woke/testing/fuzzing/fuzz_test.py
+-rw-r--r--   0        0        0    10795 2023-04-24 12:08:38.404675 woke-3.4.0/woke/testing/fuzzing/fuzzer.py
+-rw-r--r--   0        0        0     5780 2023-04-24 12:08:38.404675 woke-3.4.0/woke/testing/fuzzing/generators.py
+-rw-r--r--   0        0        0      298 2023-04-24 12:08:38.404675 woke-3.4.0/woke/testing/pytest_plugin.py
+-rw-r--r--   0        0        0      170 2023-04-24 12:08:38.404675 woke-3.4.0/woke/utils/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-11 12:18:17.001189 woke-3.4.0/woke/utils/context_managers.py
+-rw-r--r--   0        0        0      515 2023-05-11 12:18:17.001189 woke-3.4.0/woke/utils/decorators.py
+-rw-r--r--   0        0        0      158 2023-04-24 12:08:38.404675 woke-3.4.0/woke/utils/enums.py
+-rw-r--r--   0        0        0     1699 2023-04-24 12:08:38.404675 woke-3.4.0/woke/utils/file_utils.py
+-rw-r--r--   0        0        0      384 2023-05-11 12:18:17.004522 woke-3.4.0/woke/utils/keyed_default_dict.py
+-rw-r--r--   0        0        0      194 2023-04-24 12:08:38.404675 woke-3.4.0/woke/utils/networking.py
+-rw-r--r--   0        0        0     1017 2023-04-24 12:08:38.404675 woke-3.4.0/woke/utils/openzeppelin.py
+-rw-r--r--   0        0        0      630 2023-04-24 12:08:38.404675 woke-3.4.0/woke/utils/string.py
+-rw-r--r--   0        0        0     1747 2023-05-11 12:18:17.004522 woke-3.4.0/woke/utils/tee.py
+-rw-r--r--   0        0        0     3765 2023-04-24 12:08:38.404675 woke-3.4.0/woke/utils/threaded_child_watcher.py
+-rw-r--r--   0        0        0      424 2023-05-11 12:18:17.004522 woke-3.4.0/woke/utils/version.py
+-rw-r--r--   0        0        0     6129 1970-01-01 00:00:00.000000 woke-3.4.0/setup.py
+-rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 woke-3.4.0/PKG-INFO
```

### Comparing `woke-3.3.0/LICENSE` & `woke-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/README.md` & `woke-3.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 There you can also find a section on [contributing](https://ackeeblockchain.com/woke/docs/latest/contributing/).
 
 ## Features
 
 ### Testing framework
 
-See [examples](examples/testing) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.
+See [examples](examples) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.
 
 Writing tests is as simple as:
 
 ```python
 from woke.testing import *
 from pytypes.contracts.Counter import Counter
```

### Comparing `woke-3.3.0/pyproject.toml` & `woke-3.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "woke"
-version = "3.3.0"
+version = "3.4.0"
 description = "Woke is a Python-based development and testing framework for Solidity."
 license = "ISC"
 authors = ["Ackee Blockchain"]
 readme = "README.md"
 homepage = "https://ackeeblockchain.com"
 repository = "https://github.com/Ackee-Blockchain/woke"
 documentation = "https://ackeeblockchain.com/woke/docs/latest"
@@ -31,14 +31,16 @@
 parsimonious = "^0.9"
 eth-hash = { version = "^0.5.1", extras = ["pycryptodome"] }
 websocket-client = "^1.4"
 pywin32 = { version = ">= 302", platform = "win32" }
 watchdog = "~2.2.0"
 pytest = "^7"
 ipdb = "^0.13.9"
+abch_tree_sitter = "^1.1.1"
+abch_tree_sitter_solidity = "^1.2.0"
 
 pytest-asyncio = { version = "^0.17", optional = true }
 GitPython = { version = "^3.1.20", optional = true }
 
 black = { version = "^22", optional = true }
 mkdocs-material = { version = "^9", optional = true }
 mkdocstrings = { version = "^0.19", extras = ["python"], optional = true }
```

### Comparing `woke-3.3.0/woke/analysis/cfg.py` & `woke-3.4.0/woke/analysis/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import networkx as nx
 
 from woke.ast.enums import GlobalSymbolsEnum
 from woke.ast.ir.declaration.function_definition import FunctionDefinition
 from woke.ast.ir.declaration.modifier_definition import ModifierDefinition
 from woke.ast.ir.expression.function_call import FunctionCall
@@ -22,14 +22,17 @@
 from woke.ast.ir.statement.try_statement import TryStatement
 from woke.ast.ir.statement.unchecked_block import UncheckedBlock
 from woke.ast.ir.statement.while_statement import WhileStatement
 from woke.utils import StrEnum
 
 logger = logging.getLogger(__name__)
 
+# pyright: reportGeneralTypeIssues=false
+# pyright: reportOptionalSubscript=false
+
 
 class TransitionCondition(StrEnum):
     IS_TRUE = "is true"
     IS_FALSE = "is false"
     ALWAYS = "always"
     NEVER = "never"
     TRY_SUCCEEDED = "succeeded"
@@ -92,15 +95,15 @@
         for node in self.__graph.nodes:
             for stmt in node.statements:
                 self.__statements_lookup[stmt] = node
             if node.control_statement is not None:
                 self.__statements_lookup[node.control_statement] = node
 
     @property
-    def graph(self):
+    def graph(self) -> nx.DiGraph:
         return self.__graph.copy(as_view=True)
 
     @property
     def declaration(self) -> Union[FunctionDefinition, ModifierDefinition]:
         return self.__declaration
 
     @property
@@ -413,14 +416,15 @@
         if tmp == body:
             body_end = tmp
             if for_statement.loop_expression is not None:
                 body_end.__statements.append(for_statement.loop_expression)
         else:
             body_end.__statements = list(tmp.__statements)
 
+            data: Any
             for start, _, data in graph.in_edges(tmp, data=True):
                 graph.add_edge(start, body_end, condition=data["condition"])
 
             for end, _, data in graph.out_edges(tmp, data=True):
                 graph.add_edge(body_end, end, condition=data["condition"])
 
             graph.remove_node(tmp)
```

### Comparing `woke-3.3.0/woke/analysis/detectors/__init__.py` & `woke-3.4.0/woke/analysis/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/api.py` & `woke-3.4.0/woke/analysis/detectors/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,15 +569,15 @@
                 source,
                 "solidity",
                 theme=theme,
                 line_numbers=True,
                 start_line=(start_line_index + 1),
                 highlight_lines={line_index + 1},
             ),
-            title=f"{detector_result.message} \[{detector_id}]"
+            title=f"{detector_result.message} \[{detector_id}]"  # pyright: ignore reportInvalidStringEscapeSequence
             if detector_id is not None
             else detector_result.message,
             title_align="left",
             subtitle=source_unit.source_unit_name,
             subtitle_align="left",
         )
```

### Comparing `woke-3.3.0/woke/analysis/detectors/axelar/proxy_contract_id.py` & `woke-3.4.0/woke/analysis/detectors/axelar/proxy_contract_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from woke.ast.ir.declaration.contract_definition import ContractDefinition
 from woke.ast.ir.declaration.function_definition import FunctionDefinition
 from woke.ast.ir.expression.abc import ExpressionAbc
 from woke.ast.ir.expression.assignment import Assignment
 from woke.ast.ir.expression.binary_operation import BinaryOperation
 from woke.ast.ir.expression.function_call import FunctionCall
 from woke.ast.ir.expression.literal import Literal
+from woke.ast.ir.meta.identifier_path import IdentifierPathPart
+from woke.ast.ir.statement.inline_assembly import ExternalReference
 from woke.ast.ir.statement.return_statement import Return
 
 
 @detector(-12000, "axelar-proxy-contract-id")
 class AxelarProxyContractIdDetector(DetectorAbc):
     """
     Detects incorrect use of the `contractId` function in Axelar proxy and upgradeable contracts.
@@ -36,20 +38,24 @@
         self.proxies = {}
         self.upgradeables = {}
 
     def report(self) -> List[DetectorResult]:
         proxy_contracts: Dict[bytes, Set[ContractDefinition]] = {}
         for selector, fns in self.proxies.items():
             proxy_contracts[selector] = set()
-            visited: Set[ContractDefinition] = set(
+            visited: Set[
+                ContractDefinition
+            ] = set(  # pyright: ignore reportGeneralTypeIssues
                 fn.parent for fn in fns
-            )  # pyright: reportGeneralTypeIssues=false
-            queue: Deque[ContractDefinition] = deque(
+            )
+            queue: Deque[
+                ContractDefinition
+            ] = deque(  # pyright: ignore reportGeneralTypeIssues
                 fn.parent for fn in fns
-            )  # pyright: reportGeneralTypeIssues=false
+            )
 
             while len(queue) > 0:
                 contract = queue.popleft()
                 if contract.kind == ContractKind.CONTRACT and not contract.abstract:
                     proxy_contracts[selector].add(contract)
                 for child in contract.child_contracts:
                     if child not in visited and (
@@ -58,20 +64,24 @@
                     ):
                         visited.add(child)
                         queue.append(child)
 
         upgradeable_contracts: Dict[bytes, Set[ContractDefinition]] = {}
         for selector, fns in self.upgradeables.items():
             upgradeable_contracts[selector] = set()
-            visited: Set[ContractDefinition] = set(
+            visited: Set[
+                ContractDefinition
+            ] = set(  # pyright: ignore reportGeneralTypeIssues
                 fn.parent for fn in fns
-            )  # pyright: reportGeneralTypeIssues=false
-            queue: Deque[ContractDefinition] = deque(
+            )
+            queue: Deque[
+                ContractDefinition
+            ] = deque(  # pyright: ignore reportGeneralTypeIssues
                 fn.parent for fn in fns
-            )  # pyright: reportGeneralTypeIssues=false
+            )
 
             while len(queue) > 0:
                 contract = queue.popleft()
                 if contract.kind == ContractKind.CONTRACT and not contract.abstract:
                     upgradeable_contracts[selector].add(contract)
                 for child in contract.child_contracts:
                     if child not in visited and (
@@ -295,14 +305,18 @@
         if len(returns) == 1 and returns[0].expression is not None:
             expr = returns[0].expression
         else:
             ret_var = contract_id_function.return_parameters.parameters[0]
             assignments = []
 
             for ref in ret_var.references:
+                if isinstance(ref, ExternalReference):
+                    continue
+                elif isinstance(ref, IdentifierPathPart):
+                    ref = ref.underlying_node
                 assignment = ref
                 while assignment is not None:
                     if isinstance(assignment, Assignment):
                         break
                     assignment = assignment.parent
                 if assignment is None:
                     continue
```

### Comparing `woke-3.3.0/woke/analysis/detectors/balance_state_var.py` & `woke-3.4.0/woke/analysis/detectors/balance_state_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from woke.ast.ir.expression.assignment import AssignedVariablePath, Assignment
 from woke.ast.ir.expression.binary_operation import BinaryOperation
 from woke.ast.ir.expression.function_call import FunctionCall
 from woke.ast.ir.expression.function_call_options import FunctionCallOptions
 from woke.ast.ir.expression.identifier import Identifier
 from woke.ast.ir.expression.member_access import MemberAccess
 from woke.ast.ir.expression.tuple_expression import TupleExpression
+from woke.ast.ir.meta.source_unit import SourceUnit
 from woke.ast.ir.statement.abc import StatementAbc
 from woke.ast.ir.statement.variable_declaration_statement import (
     VariableDeclarationStatement,
 )
 
 logger = logging.getLogger(__name__)
 _recursion_guard = set()
@@ -92,15 +93,15 @@
 
     if len(assigned_vars) > 1 or len(next(iter(assigned_vars))) > 1:
         # currently not supported
         logger.debug(f"Complex assignment not supported: {statement.source}")
         return ret
 
     assigned_var = next(iter(assigned_vars))[0]
-    assert assigned_var != "IndexAccess"
+    assert assigned_var != "IndexAccess" and not isinstance(assigned_var, SourceUnit)
     assigned_var_statement = None
     function_def = None
     node = assigned_var
     while node is not None:
         if isinstance(node, StatementAbc) and assigned_var_statement is None:
             assigned_var_statement = node
         if isinstance(node, FunctionDefinition):
```

### Comparing `woke-3.3.0/woke/analysis/detectors/bug_empty_byte_array_copy.py` & `woke-3.4.0/woke/analysis/detectors/bug_empty_byte_array_copy.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/call_options_not_called.py` & `woke-3.4.0/woke/analysis/detectors/call_options_not_called.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/missing_return.py` & `woke-3.4.0/woke/analysis/detectors/missing_return.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/msg_value_nonpayable_function.py` & `woke-3.4.0/woke/analysis/detectors/msg_value_nonpayable_function.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py` & `woke-3.4.0/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,16 +205,19 @@
         }:
             assert len(node.arguments) >= 1
             encoded_types = [arg.type for arg in node.arguments[1:]]
         elif t.kind == FunctionTypeKind.ABI_ENCODE_CALL:
             assert len(node.arguments) == 2
             if isinstance(node.arguments[1], TupleExpression):
                 encoded_types = [
-                    arg.type for arg in node.arguments[1].components
-                ]  # pyright: reportGeneralTypeIssues=false
+                    arg.type if arg is not None else None
+                    for arg in node.arguments[
+                        1
+                    ].components  # pyright: ignore reportGeneralTypeIssues
+                ]
             elif (
                 isinstance(node.arguments[1], FunctionCall)
                 and node.arguments[1].kind == FunctionCallKind.STRUCT_CONSTRUCTOR_CALL
             ):
                 # probably always created in memory, not calldata
                 return
             else:
@@ -225,13 +228,15 @@
         else:
             return
 
         # ABI encoder v2 must be enabled
         if not abi_encoder_v2_enabled(node):
             return
 
-        if types_meet_requirements(encoded_types):  # type: ignore
+        if types_meet_requirements(
+            encoded_types  # pyright: ignore reportGeneralTypeIssues
+        ):
             self._detections.add(
                 DetectorResult(
                     node, "Found head overflow calldata tuple reencoding compiler bug"
                 )
             )
```

### Comparing `woke-3.3.0/woke/analysis/detectors/ownable.py` & `woke-3.4.0/woke/analysis/detectors/ownable.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,34 +293,42 @@
             queue = deque([block])
             reached_start = False
 
             while len(queue) > 0:
                 block = queue.popleft()
                 from_: CfgBlock
                 condition: Tuple[TransitionCondition, Optional[ExpressionAbc]]
-                for from_, _, data in graph.in_edges(block, data=True):
+                for (
+                    from_,
+                    _,
+                    data,
+                ) in graph.in_edges(  # pyright: ignore reportGeneralTypeIssues
+                    block, data=True  # pyright: ignore reportGeneralTypeIssues
+                ):
                     if from_ in visited:
                         continue
-                    condition = data["condition"]
+                    condition = data[  # pyright: ignore reportOptionalSubscript
+                        "condition"
+                    ]
                     if (
                         (condition[0] == TransitionCondition.NEVER)
                         or (
                             condition[0] == TransitionCondition.IS_TRUE
                             and condition[1] is not None
                             and expression_is_only_owner(
-                                condition[1],
+                                condition[1],  # pyright: ignore reportGeneralTypeIssues
                                 set(),
-                                check_only_eoa=check_only_eoa,  # pyright: reportGeneralTypeIssues=false
+                                check_only_eoa=check_only_eoa,
                             )
                         )
                         or (
                             condition[0] == TransitionCondition.IS_FALSE
                             and condition[1] is not None
                             and expression_is_only_owner(
-                                condition[1],  # pyright: reportGeneralTypeIssues=false
+                                condition[1],  # pyright: ignore reportGeneralTypeIssues
                                 set(),
                                 check_only_eoa=check_only_eoa,
                                 inverted=True,
                             )
                         )
                     ):
                         continue
```

### Comparing `woke-3.3.0/woke/analysis/detectors/proxy_contract_selector_clashes.py` & `woke-3.4.0/woke/analysis/detectors/proxy_contract_selector_clashes.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/reentrancy.py` & `woke-3.4.0/woke/analysis/detectors/reentrancy.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,30 +178,30 @@
             ret.update(s.modifies_state)
         if start.control_statement is not None:
             ret.update(start.control_statement.modifies_state)
 
     queue = deque([])
     visited: Set[CfgBlock] = set()
 
-    for _, to in graph.out_edges(start):
+    for _, to in graph.out_edges(start):  # pyright: ignore reportGeneralTypeIssues
         if to in visited:
             continue
         if not nx.has_path(graph, to, cfg.end_block):
             continue
         queue.append(to)
 
     while len(queue):
         block = queue.popleft()
         for s in block.statements:
             ret.update(s.modifies_state)
         if block.control_statement is not None:
             ret.update(block.control_statement.modifies_state)
 
         to: CfgBlock
-        for _, to in graph.out_edges(block):
+        for _, to in graph.out_edges(block):  # pyright: ignore reportGeneralTypeIssues
             if to in visited:
                 continue
             if not nx.has_path(graph, to, cfg.end_block):
                 continue
 
             visited.add(to)
             queue.append(to)
```

### Comparing `woke-3.3.0/woke/analysis/detectors/unchecked_return_value.py` & `woke-3.4.0/woke/analysis/detectors/unchecked_return_value.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/unsafe_delegatecall.py` & `woke-3.4.0/woke/analysis/detectors/unsafe_delegatecall.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/unsafe_selfdestruct.py` & `woke-3.4.0/woke/analysis/detectors/unsafe_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/unsafe_tx_origin.py` & `woke-3.4.0/woke/analysis/detectors/unsafe_tx_origin.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/unused_contract.py` & `woke-3.4.0/woke/analysis/detectors/unused_contract.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/analysis/detectors/utils.py` & `woke-3.4.0/woke/analysis/detectors/utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/enums.py` & `woke-3.4.0/woke/ast/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,15 @@
     BYZANTIUM = "byzantium"
     CONSTANTINOPLE = "constantinople"
     PETERSBURG = "petersburg"
     ISTANBUL = "istanbul"
     BERLIN = "berlin"
     LONDON = "london"
     PARIS = "paris"
+    SHANGHAI = "shanghai"
 
 
 class InlineAssemblySuffix(StrEnum):
     SLOT = "slot"
     OFFSET = "offset"
     LENGTH = "length"
     ADDRESS = "address"
```

### Comparing `woke-3.3.0/woke/ast/ir/abc.py` & `woke-3.4.0/woke/ast/ir/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Each IR node is associated with a [source code location][woke.ast.ir.abc.IrAbc.byte_location] in a [source file][woke.ast.ir.abc.IrAbc.file].
     This means that each IR node has a corresponding (typically non-empty) Solidity or Yul [source code][woke.ast.ir.abc.IrAbc.source].
 
     !!! info
         Yul IR nodes can have empty source code. In the case of Solidity IR nodes, this should not happen.
 
     """
+
     _file: Path
     _source: bytes
     _ast_node: SolcOrYulNode
     _version_ranges: SolidityVersionRanges
     _parent: Optional[IrAbc]
     _depth: int
     _cu_hash: bytes
@@ -146,14 +147,15 @@
         return self._source.decode("utf-8")
 
 
 class SolidityAbc(IrAbc, ABC):
     """
     Abstract base class for all Solidity IR nodes.
     """
+
     _ast_node: SolcNode
 
     def __init__(
         self, init: IrInitTuple, solc_node: SolcNode, parent: Optional[SolidityAbc]
     ):
         super().__init__(init, solc_node, parent)
         self._reference_resolver.register_node(self, solc_node.id, self._cu_hash)
```

### Comparing `woke-3.3.0/woke/ast/ir/declaration/abc.py` & `woke-3.4.0/woke/ast/ir/declaration/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/declaration/contract_definition.py` & `woke-3.4.0/woke/ast/ir/declaration/contract_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,28 +88,33 @@
     _events: List[EventDefinition]
     _functions: List[FunctionDefinition]
     _modifiers: List[ModifierDefinition]
     _structs: List[StructDefinition]
     _user_defined_value_types: List[UserDefinedValueTypeDefinition]
     _using_for_directives: List[UsingForDirective]
     _declared_variables: List[VariableDeclaration]
+    _used_events: List[AstNodeId]
+    # _internal_function_ids
 
     _child_contracts: Set[ContractDefinition]
 
     def __init__(
         self, init: IrInitTuple, contract: SolcContractDefinition, parent: SourceUnit
     ):
         super().__init__(init, contract, parent)
         self._abstract = contract.abstract
         self._kind = contract.contract_kind
         self._fully_implemented = contract.fully_implemented
         self._linearized_base_contracts = list(contract.linearized_base_contracts)
         self._used_errors = (
             list(contract.used_errors) if contract.used_errors is not None else []
         )
+        self._used_events = (
+            list(contract.used_events) if contract.used_events is not None else []
+        )
 
         if contract.documentation is None:
             self._documentation = None
         elif isinstance(contract.documentation, SolcStructuredDocumentation):
             self._documentation = StructuredDocumentation(
                 init, contract.documentation, self
             )
@@ -286,15 +291,15 @@
 
         Returns:
             `True` if the contract is abstract, `False` otherwise.
         """
         return self._abstract
 
     @property
-    def base_contracts(self) -> Tuple[InheritanceSpecifier]:
+    def base_contracts(self) -> Tuple[InheritanceSpecifier, ...]:
         """
         Returns base contracts as specified in the source code. Does not return all base contracts (recursively).
         !!! example
             `A1` lists the interface `I` as a base contract.
 
             `A2` lists the interface `I` as a base contract.
 
@@ -332,118 +337,131 @@
         Is `None` when a file that imports this contract cannot be compiled. This may happen in the LSP server where partial project analysis is supported.
         Returns:
             `True` if all functions and modifiers of the contract are implemented, `False` otherwise.
         """
         return self._fully_implemented
 
     @property
-    def linearized_base_contracts(self) -> Tuple[ContractDefinition]:
+    def linearized_base_contracts(self) -> Tuple[ContractDefinition, ...]:
         """
         Returns:
             C3 linearized list of all base contracts.
         """
         base_contracts = []
         for base_contract in self._linearized_base_contracts:
             node = self._reference_resolver.resolve_node(base_contract, self._cu_hash)
             assert isinstance(node, ContractDefinition)
             base_contracts.append(node)
         return tuple(base_contracts)
 
     @property
-    def used_errors(self) -> Tuple[ErrorDefinition]:
+    def used_errors(self) -> Tuple[ErrorDefinition, ...]:
         """
         Returns:
             Errors used in the contract.
         """
         used_errors = []
         for error in self._used_errors:
             node = self._reference_resolver.resolve_node(error, self._cu_hash)
             assert isinstance(node, ErrorDefinition)
             used_errors.append(node)
         return tuple(used_errors)
 
     @property
+    def used_events(self) -> Tuple[EventDefinition, ...]:
+        """
+        Returns:
+            Events emitted by the contract as well as all events defined and inherited by the contract.
+        """
+        used_events = []
+        for event in self._used_events:
+            node = self._reference_resolver.resolve_node(event, self._cu_hash)
+            assert isinstance(node, EventDefinition)
+            used_events.append(node)
+        return tuple(used_events)
+
+    @property
     def documentation(self) -> Optional[Union[StructuredDocumentation, str]]:
         """
         Of [StructuredDocumentation][woke.ast.ir.meta.structured_documentation.StructuredDocumentation] type since Solidity 0.6.3.
         Returns:
             [NatSpec](https://docs.soliditylang.org/en/latest/natspec-format.html) documentation of this contract, if any.
         """
         return self._documentation
 
     @property
     def compilation_info(self) -> Optional[SolcOutputContractInfo]:
         return self._compilation_info
 
     @property
-    def enums(self) -> Tuple[EnumDefinition]:
+    def enums(self) -> Tuple[EnumDefinition, ...]:
         """
         Returns:
             Enum definitions contained in this contract.
         """
         return tuple(self._enums)
 
     @property
-    def errors(self) -> Tuple[ErrorDefinition]:
+    def errors(self) -> Tuple[ErrorDefinition, ...]:
         """
         Returns:
             Error definitions contained in this contract.
         """
         return tuple(self._errors)
 
     @property
-    def events(self) -> Tuple[EventDefinition]:
+    def events(self) -> Tuple[EventDefinition, ...]:
         """
         Returns:
             Event definitions contained in this contract.
         """
         return tuple(self._events)
 
     @property
-    def functions(self) -> Tuple[FunctionDefinition]:
+    def functions(self) -> Tuple[FunctionDefinition, ...]:
         """
         Returns:
             Function definitions contained in this contract.
         """
         return tuple(self._functions)
 
     @property
-    def modifiers(self) -> Tuple[ModifierDefinition]:
+    def modifiers(self) -> Tuple[ModifierDefinition, ...]:
         """
         Returns:
             Modifier definitions contained in this contract.
         """
         return tuple(self._modifiers)
 
     @property
-    def structs(self) -> Tuple[StructDefinition]:
+    def structs(self) -> Tuple[StructDefinition, ...]:
         """
         Returns:
             Struct definitions contained in this contract.
         """
         return tuple(self._structs)
 
     @property
-    def user_defined_value_types(self) -> Tuple[UserDefinedValueTypeDefinition]:
+    def user_defined_value_types(self) -> Tuple[UserDefinedValueTypeDefinition, ...]:
         """
         Returns:
             User defined value type definitions contained in this contract.
         """
         return tuple(self._user_defined_value_types)
 
     @property
-    def using_for_directives(self) -> Tuple[UsingForDirective]:
+    def using_for_directives(self) -> Tuple[UsingForDirective, ...]:
         """
         Returns:
             Using for directives contained in this contract.
         """
         return tuple(self._using_for_directives)
 
     @property
-    def declared_variables(self) -> Tuple[VariableDeclaration]:
+    def declared_variables(self) -> Tuple[VariableDeclaration, ...]:
         """
         Returns:
             Variable declarations contained in this contract.
         """
         return tuple(self._declared_variables)
 
     def declarations_iter(self) -> Iterator[DeclarationAbc]:
```

### Comparing `woke-3.3.0/woke/ast/ir/declaration/enum_definition.py` & `woke-3.4.0/woke/ast/ir/declaration/enum_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import logging
 import re
 from functools import lru_cache
-from typing import TYPE_CHECKING, Iterator, List, Tuple, Union
+from typing import TYPE_CHECKING, Iterator, List, Optional, Tuple, Union
 
 from woke.ast.nodes import SolcEnumDefinition
 
 from ..abc import IrAbc, SolidityAbc
+from ..meta.structured_documentation import StructuredDocumentation
 from ..utils import IrInitTuple
 from .abc import DeclarationAbc
 from .enum_value import EnumValue
 
 if TYPE_CHECKING:
     from ..meta.source_unit import SourceUnit
     from .contract_definition import ContractDefinition
@@ -31,24 +32,30 @@
     """
 
     _ast_node: SolcEnumDefinition
     _parent: Union[ContractDefinition, SourceUnit]
 
     _canonical_name: str
     _values: List[EnumValue]
+    _documentation: Optional[StructuredDocumentation]
 
     def __init__(
         self, init: IrInitTuple, enum: SolcEnumDefinition, parent: SolidityAbc
     ):
         super().__init__(init, enum, parent)
         self._canonical_name = enum.canonical_name
 
         self._values = []
         for value in enum.members:
             self._values.append(EnumValue(init, value, self))
+        self._documentation = (
+            StructuredDocumentation(init, enum.documentation, self)
+            if enum.documentation is not None
+            else None
+        )
 
     def __iter__(self) -> Iterator[IrAbc]:
         yield self
         for value in self._values:
             yield from value
 
     def _parse_name_location(self) -> Tuple[int, int]:
@@ -83,13 +90,22 @@
             f"enum {self.name}"
             + " {\n"
             + ",\n".join(f"    {value.name}" for value in self._values)
             + "\n}"
         )
 
     @property
-    def values(self) -> Tuple[EnumValue]:
+    def values(self) -> Tuple[EnumValue, ...]:
         """
         Returns:
             Enum values defined in this enum.
         """
         return tuple(self._values)
+
+    @property
+    def documentation(self) -> Optional[StructuredDocumentation]:
+        """
+        Added in Solidity 0.8.20.
+        Returns:
+            [NatSpec](https://docs.soliditylang.org/en/latest/natspec-format.html) documentation string, if any.
+        """
+        return self._documentation
```

### Comparing `woke-3.3.0/woke/ast/ir/declaration/enum_value.py` & `woke-3.4.0/woke/ast/ir/declaration/enum_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     !!! example
         `GoLeft`, `GoRight`, `GoStraight`, `SitStill` in the following enum definition:
         ```solidity
         enum ActionChoices { GoLeft, GoRight, GoStraight, SitStill }
         ```
     """
+
     _ast_node: SolcEnumValue
     _parent: EnumDefinition
 
     def __init__(self, init: IrInitTuple, value: SolcEnumValue, parent: SolidityAbc):
         super().__init__(init, value, parent)
 
     def _parse_name_location(self) -> Tuple[int, int]:
```

### Comparing `woke-3.3.0/woke/ast/ir/declaration/error_definition.py` & `woke-3.4.0/woke/ast/ir/declaration/error_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __init__(
         self, init: IrInitTuple, error: SolcErrorDefinition, parent: SolidityAbc
     ):
         super().__init__(init, error, parent)
         self._parameters = ParameterList(init, error.parameters, self)
         self._documentation = (
             StructuredDocumentation(init, error.documentation, self)
-            if error.documentation
+            if error.documentation is not None
             else None
         )
         self._error_selector = (
             bytes.fromhex(error.error_selector) if error.error_selector else None
         )
         self._used_in = []
 
@@ -131,13 +131,13 @@
                 param.type.abi_type() for param in self.parameters.parameters
             )
             signature += ")"
             h = keccak.new(data=signature.encode("utf-8"), digest_bits=256)
             return h.digest()[:4]
 
     @property
-    def used_in(self) -> Tuple[ContractDefinition]:
+    def used_in(self) -> Tuple[ContractDefinition, ...]:
         """
         Returns:
             List of contracts where the error is used.
         """
         return tuple(self._used_in)
```

### Comparing `woke-3.3.0/woke/ast/ir/declaration/event_definition.py` & `woke-3.4.0/woke/ast/ir/declaration/event_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/declaration/function_definition.py` & `woke-3.4.0/woke/ast/ir/declaration/function_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         """
         Returns:
             Kind of the function.
         """
         return self._kind
 
     @property
-    def modifiers(self) -> Tuple[ModifierInvocation]:
+    def modifiers(self) -> Tuple[ModifierInvocation, ...]:
         """
         Also includes base constructor invocations.
         !!! example
             Both `:::solidity ERC20Token("My Token", "MTK", msg.sender, 10 ** 18)` and `initializer` are listed by this property.
             ```solidity
             contract MyToken is ERC20Token {
                 constructor() ERC20Token("My Token", "MTK", msg.sender, 10 ** 18) initializer {}
@@ -411,15 +411,15 @@
         """
         Returns:
             Visibility of the function.
         """
         return self._visibility
 
     @property
-    def base_functions(self) -> Tuple[FunctionDefinition]:
+    def base_functions(self) -> Tuple[FunctionDefinition, ...]:
         """
         !!! example
             `A.foo` on lines 6-8 lists `I.foo` on line 2 as a base function.
 
             `B.foo` on lines 12-14 lists only `A.foo` on lines 6-8 as a base function.
             ```solidity linenums="1"
             interface I {
```

### Comparing `woke-3.3.0/woke/ast/ir/declaration/modifier_definition.py` & `woke-3.4.0/woke/ast/ir/declaration/modifier_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
         """
         Returns:
             Visibility of the modifier.
         """
         return self._visibility
 
     @property
-    def base_modifiers(self) -> Tuple[ModifierDefinition]:
+    def base_modifiers(self) -> Tuple[ModifierDefinition, ...]:
         """
         !!! example
             `B.mod` on lines 6-8 lists `A.mod` on line 2 as a base modifier.
 
             `C.mod` on lines 12-14 lists only `B.mod` on lines 6-8 as a base modifier.
             ```solidity linenums="1"
             abstract contract A {
```

### Comparing `woke-3.3.0/woke/ast/ir/declaration/struct_definition.py` & `woke-3.4.0/woke/ast/ir/declaration/struct_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import re
 from functools import lru_cache
-from typing import TYPE_CHECKING, Iterator, List, Tuple, Union
+from typing import TYPE_CHECKING, Iterator, List, Optional, Tuple, Union
 
+from ..meta.structured_documentation import StructuredDocumentation
 from .abc import DeclarationAbc
 
 if TYPE_CHECKING:
     from .contract_definition import ContractDefinition
     from ..meta.source_unit import SourceUnit
 
 from woke.ast.enums import Visibility
@@ -32,14 +33,15 @@
 
     _ast_node: SolcStructDefinition
     _parent: Union[ContractDefinition, SourceUnit]
 
     _canonical_name: str
     _members: List[VariableDeclaration]
     _visibility: Visibility
+    _documentation: Optional[StructuredDocumentation]
 
     def __init__(
         self,
         init: IrInitTuple,
         struct_definition: SolcStructDefinition,
         parent: SolidityAbc,
     ):
@@ -47,14 +49,19 @@
         self._canonical_name = struct_definition.canonical_name
         # TODO scope
         self._visibility = struct_definition.visibility
 
         self._members = []
         for member in struct_definition.members:
             self._members.append(VariableDeclaration(init, member, self))
+        self._documentation = (
+            StructuredDocumentation(init, struct_definition.documentation, self)
+            if struct_definition.documentation is not None
+            else None
+        )
 
     def __iter__(self) -> Iterator[IrAbc]:
         yield self
         for member in self._members:
             yield from member
 
     def _parse_name_location(self) -> Tuple[int, int]:
@@ -89,13 +96,22 @@
             f"struct {self.name}"
             + " {\n"
             + ";\n".join(f"    {member.declaration_string}" for member in self._members)
             + ";\n}"
         )
 
     @property
-    def members(self) -> Tuple[VariableDeclaration]:
+    def members(self) -> Tuple[VariableDeclaration, ...]:
         """
         Returns:
             Tuple of member variable declarations.
         """
         return tuple(self._members)
+
+    @property
+    def documentation(self) -> Optional[StructuredDocumentation]:
+        """
+        Added in Solidity 0.8.20.
+        Returns:
+            [NatSpec](https://docs.soliditylang.org/en/latest/natspec-format.html) documentation string, if any.
+        """
+        return self._documentation
```

### Comparing `woke-3.3.0/woke/ast/ir/declaration/user_defined_value_type_definition.py` & `woke-3.4.0/woke/ast/ir/declaration/user_defined_value_type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/declaration/variable_declaration.py` & `woke-3.4.0/woke/ast/ir/declaration/variable_declaration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import logging
 import re
+from collections import deque
 from functools import lru_cache, partial
-from typing import TYPE_CHECKING, Iterator, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Deque, Iterator, List, Optional, Set, Tuple, Union
 
 from woke.ast.enums import DataLocation, Mutability, Visibility
 from woke.ast.ir.abc import IrAbc, SolidityAbc
 from woke.ast.ir.declaration.abc import DeclarationAbc
 from woke.ast.ir.expression.abc import ExpressionAbc
 from woke.ast.ir.meta.structured_documentation import StructuredDocumentation
 from woke.ast.ir.type_name.abc import TypeNameAbc
@@ -19,16 +20,22 @@
 from ..meta.override_specifier import OverrideSpecifier
 from ..reference_resolver import CallbackParams
 
 if TYPE_CHECKING:
     from ..declaration.contract_definition import ContractDefinition
     from ..declaration.function_definition import FunctionDefinition
     from ..declaration.struct_definition import StructDefinition
+    from ..expression.binary_operation import BinaryOperation
+    from ..expression.identifier import Identifier
+    from ..expression.member_access import MemberAccess
+    from ..expression.unary_operation import UnaryOperation
+    from ..meta.identifier_path import IdentifierPathPart
     from ..meta.parameter_list import ParameterList
     from ..meta.source_unit import SourceUnit
+    from ..statement.inline_assembly import ExternalReference
     from ..statement.variable_declaration_statement import VariableDeclarationStatement
 
 
 logger = logging.getLogger(__name__)
 
 
 class VariableDeclaration(DeclarationAbc):
@@ -216,14 +223,53 @@
             )
         )
         match = VARIABLE_RE.search(source_without_value)
         assert match
         byte_start = self._ast_node.src.byte_offset
         return byte_start + match.start("name"), byte_start + match.end("name")
 
+    def get_all_references(
+        self, include_declarations: bool
+    ) -> Iterator[
+        Union[
+            DeclarationAbc,
+            Identifier,
+            IdentifierPathPart,
+            MemberAccess,
+            ExternalReference,
+            UnaryOperation,
+            BinaryOperation,
+        ]
+    ]:
+        from .function_definition import FunctionDefinition
+
+        processed_declarations: Set[Union[FunctionDefinition, VariableDeclaration]] = {
+            self
+        }
+        declarations_queue: Deque[
+            Union[FunctionDefinition, VariableDeclaration]
+        ] = deque([self])
+
+        while declarations_queue:
+            declaration = declarations_queue.pop()
+            if include_declarations:
+                yield declaration
+            yield from declaration.references
+
+            if isinstance(declaration, (FunctionDefinition, VariableDeclaration)):
+                for base_function in declaration.base_functions:
+                    if base_function not in processed_declarations:
+                        declarations_queue.append(base_function)
+                        processed_declarations.add(base_function)
+            if isinstance(declaration, FunctionDefinition):
+                for child_function in declaration.child_functions:
+                    if child_function not in processed_declarations:
+                        declarations_queue.append(child_function)
+                        processed_declarations.add(child_function)
+
     @property
     def parent(
         self,
     ) -> Union[
         ContractDefinition,
         ParameterList,
         SourceUnit,
@@ -324,15 +370,15 @@
         """
         Returns:
             Visibility of the variable.
         """
         return self._visibility
 
     @property
-    def base_functions(self) -> Tuple[FunctionDefinition]:
+    def base_functions(self) -> Tuple[FunctionDefinition, ...]:
         """
         !!! example
             `C.foo` in line 6 lists `I.foo` in line 2 as a base function.
             ```solidity linenums="1"
             interface I {
                 function foo(uint, bool) external returns(uint);
             }
```

### Comparing `woke-3.3.0/woke/ast/ir/expression/abc.py` & `woke-3.4.0/woke/ast/ir/expression/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/expression/assignment.py` & `woke-3.4.0/woke/ast/ir/expression/assignment.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 
 from woke.ast.enums import AssignmentOperator, ModifiesStateFlag
 from woke.ast.ir.abc import IrAbc, SolidityAbc
 from woke.ast.ir.utils import IrInitTuple
 from woke.ast.nodes import SolcAssignment
 
 from ..declaration.abc import DeclarationAbc
+from ..meta.source_unit import SourceUnit
 from .abc import ExpressionAbc
 from .conditional import Conditional
 from .identifier import Identifier
 from .index_access import IndexAccess
 from .member_access import MemberAccess
 from .tuple_expression import TupleExpression
 
-AssignedVariablePath = Tuple[Union[DeclarationAbc, Literal["IndexAccess"]], ...]
+AssignedVariablePath = Tuple[
+    Union[DeclarationAbc, SourceUnit, Literal["IndexAccess"]], ...
+]
 
 
 class Assignment(ExpressionAbc):
     """
     TBD
     """
 
@@ -83,24 +86,24 @@
         def resolve_node(node: ExpressionAbc) -> Set[AssignedVariablePath]:
             if isinstance(node, Conditional):
                 return resolve_node(node.true_expression) | resolve_node(
                     node.false_expression
                 )
             elif isinstance(node, Identifier):
                 referenced_declaration = node.referenced_declaration
-                assert isinstance(referenced_declaration, DeclarationAbc)
+                assert isinstance(referenced_declaration, (DeclarationAbc, SourceUnit))
                 return {(referenced_declaration,)}
             elif isinstance(node, IndexAccess):
                 return {
                     path + ("IndexAccess",)
                     for path in resolve_node(node.base_expression)
                 }
             elif isinstance(node, MemberAccess):
                 referenced_declaration = node.referenced_declaration
-                assert isinstance(referenced_declaration, DeclarationAbc)
+                assert isinstance(referenced_declaration, (DeclarationAbc, SourceUnit))
                 return {
                     path + (referenced_declaration,)
                     for path in resolve_node(node.expression)
                 }
             else:
                 assert False, f"Unexpected node type: {type(node)}\n{self.source}"
```

### Comparing `woke-3.3.0/woke/ast/ir/expression/binary_operation.py` & `woke-3.4.0/woke/ast/ir/expression/binary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/expression/conditional.py` & `woke-3.4.0/woke/ast/ir/expression/conditional.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/expression/elementary_type_name_expression.py` & `woke-3.4.0/woke/ast/ir/expression/elementary_type_name_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/expression/function_call.py` & `woke-3.4.0/woke/ast/ir/expression/function_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,27 +70,27 @@
         return self._parent
 
     @property
     def kind(self) -> FunctionCallKind:
         return self._kind
 
     @property
-    def names(self) -> Tuple[str]:
+    def names(self) -> Tuple[str, ...]:
         return tuple(self._names)
 
     @property
     def try_call(self) -> bool:
         return self._try_call
 
     @property
     def expression(self) -> ExpressionAbc:
         return self._expression
 
     @property
-    def arguments(self) -> Tuple[ExpressionAbc]:
+    def arguments(self) -> Tuple[ExpressionAbc, ...]:
         return tuple(self._arguments)
 
     @property
     @lru_cache(maxsize=2048)
     def function_called(
         self,
     ) -> Optional[
```

### Comparing `woke-3.3.0/woke/ast/ir/expression/function_call_options.py` & `woke-3.4.0/woke/ast/ir/expression/function_call_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,19 @@
         return self._parent
 
     @property
     def expression(self) -> ExpressionAbc:
         return self._expression
 
     @property
-    def names(self) -> Tuple[str]:
+    def names(self) -> Tuple[str, ...]:
         return tuple(self._names)
 
     @property
-    def options(self) -> Tuple[ExpressionAbc]:
+    def options(self) -> Tuple[ExpressionAbc, ...]:
         return tuple(self._options)
 
     @property
     def is_ref_to_state_variable(self) -> bool:
         return False
 
     @property
```

### Comparing `woke-3.3.0/woke/ast/ir/expression/index_access.py` & `woke-3.4.0/woke/ast/ir/expression/index_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/expression/index_range_access.py` & `woke-3.4.0/woke/ast/ir/expression/index_range_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/expression/literal.py` & `woke-3.4.0/woke/ast/ir/expression/literal.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/expression/member_access.py` & `woke-3.4.0/woke/ast/ir/expression/member_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from woke.ast.enums import GlobalSymbolsEnum, ModifiesStateFlag
 from woke.ast.ir.abc import IrAbc, SolidityAbc
 from woke.ast.ir.declaration.abc import DeclarationAbc
 from woke.ast.ir.declaration.enum_definition import EnumDefinition
 from woke.ast.ir.declaration.variable_declaration import VariableDeclaration
 from woke.ast.ir.expression.abc import ExpressionAbc
 from woke.ast.ir.expression.identifier import Identifier
+from woke.ast.ir.meta.import_directive import ImportDirective
+from woke.ast.ir.meta.source_unit import SourceUnit
 from woke.ast.ir.reference_resolver import CallbackParams
 from woke.ast.ir.utils import IrInitTuple
 from woke.ast.nodes import AstNodeId, SolcMemberAccess
 from woke.ast.types import (
     Address,
     Array,
     Bytes,
@@ -51,15 +53,17 @@
         self._expression = ExpressionAbc.from_ast(init, member_access.expression, self)
         assert self._expression.byte_location[0] == self.byte_location[0]
         assert self._expression.byte_location[1] < self.byte_location[1]
 
         self._member_name = member_access.member_name
         self._referenced_declaration_id = member_access.referenced_declaration
 
-        self._reference_resolver.register_post_process_callback(self._post_process)
+        self._reference_resolver.register_post_process_callback(
+            self._post_process, priority=-1
+        )
 
     def __iter__(self) -> Iterator[IrAbc]:
         yield self
         yield from self._expression
 
     def _post_process(self, callback_params: CallbackParams):
         # workaround for enum value bug in Solidity versions prior to 0.8.2
@@ -329,21 +333,39 @@
             self._reference_resolver.register_global_symbol_reference(
                 global_symbol, self
             )
             self._reference_resolver.register_destroy_callback(
                 self.file, partial(self._destroy, global_symbol)
             )
         else:
-            referenced_declaration = self.referenced_declaration
-            assert isinstance(referenced_declaration, DeclarationAbc)
-            referenced_declaration.register_reference(self)
-            self._reference_resolver.register_destroy_callback(
-                self.file, partial(self._destroy, referenced_declaration)
+            node = self._reference_resolver.resolve_node(
+                self._referenced_declaration_id, self._cu_hash
             )
 
+            if isinstance(node, DeclarationAbc):
+                node.register_reference(self)
+                self._reference_resolver.register_destroy_callback(
+                    self.file, partial(self._destroy, node)
+                )
+            elif isinstance(node, ImportDirective):
+                # make this node to reference the source unit directly
+                assert node.unit_alias is not None
+                source_unit = callback_params.source_units[node.imported_file]
+                node_path_order = self._reference_resolver.get_node_path_order(
+                    AstNodeId(source_unit.ast_node_id),
+                    source_unit.cu_hash,
+                )
+                self._referenced_declaration_id = (
+                    self._reference_resolver.get_ast_id_from_cu_node_path_order(
+                        node_path_order, self.cu_hash
+                    )
+                )
+            else:
+                raise TypeError(f"Unexpected type: {type(node)}")
+
     def _destroy(
         self, referenced_declaration: Union[GlobalSymbolsEnum, DeclarationAbc]
     ) -> None:
         if isinstance(referenced_declaration, GlobalSymbolsEnum):
             self._reference_resolver.unregister_global_symbol_reference(
                 referenced_declaration, self
             )
@@ -373,23 +395,25 @@
         match = MEMBER_RE.match(self._source[relative_expression_end:])
         assert match
         return self._expression.byte_location[1] + match.start(
             "member"
         ), self._expression.byte_location[1] + match.end("member")
 
     @property
-    def referenced_declaration(self) -> Union[DeclarationAbc, GlobalSymbolsEnum]:
+    def referenced_declaration(
+        self,
+    ) -> Union[DeclarationAbc, GlobalSymbolsEnum, SourceUnit]:
         assert self._referenced_declaration_id is not None
         if self._referenced_declaration_id < 0:
             return GlobalSymbolsEnum(self._referenced_declaration_id)
 
         node = self._reference_resolver.resolve_node(
             self._referenced_declaration_id, self._cu_hash
         )
-        assert isinstance(node, DeclarationAbc)
+        assert isinstance(node, (DeclarationAbc, SourceUnit))
         return node
 
     @property
     @lru_cache(maxsize=2048)
     def is_ref_to_state_variable(self) -> bool:
         referenced_declaration = self.referenced_declaration
         return (
```

### Comparing `woke-3.3.0/woke/ast/ir/expression/new_expression.py` & `woke-3.4.0/woke/ast/ir/expression/new_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/expression/tuple_expression.py` & `woke-3.4.0/woke/ast/ir/expression/tuple_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         return self._parent
 
     @property
     def is_inline_array(self) -> bool:
         return self._is_inline_array
 
     @property
-    def components(self) -> Tuple[Optional[ExpressionAbc]]:
+    def components(self) -> Tuple[Optional[ExpressionAbc], ...]:
         return tuple(self._components)
 
     @property
     @lru_cache(maxsize=2048)
     def is_ref_to_state_variable(self) -> bool:
         return any(
             component.is_ref_to_state_variable
```

### Comparing `woke-3.3.0/woke/ast/ir/expression/unary_operation.py` & `woke-3.4.0/woke/ast/ir/expression/unary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/meta/identifier_path.py` & `woke-3.4.0/woke/ast/ir/meta/identifier_path.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import re
+from collections import deque
 from functools import partial
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Deque, Optional, Set, Tuple, Union
 
 if TYPE_CHECKING:
     from .inheritance_specifier import InheritanceSpecifier
     from .modifier_invocation import ModifierInvocation
     from .override_specifier import OverrideSpecifier
     from .source_unit import SourceUnit
     from .using_for_directive import UsingForDirective
@@ -27,75 +28,50 @@
 class IdentifierPathPart:
     """
     A class representing a part of an identifier path. Is almost the same as [Identifier][woke.ast.ir.expression.identifier.Identifier], but it is not generated in the AST output of the compiler and so it is not an IR node.
     """
 
     _reference_resolver: ReferenceResolver
     _underlying_node: Union[IdentifierPath, UserDefinedTypeName]
-    _path_referenced_declaration_id: AstNodeId
-    _path_index: int
     _referenced_declaration_id: Optional[AstNodeId]
     _cu_hash: bytes
     _file: Path
     _byte_location: Tuple[int, int]
     _name: str
 
     def __init__(
         self,
         underlying_node: Union[IdentifierPath, UserDefinedTypeName],
-        init: IrInitTuple,
         byte_location: Tuple[int, int],
         name: str,
-        path_referenced_declaration_id: AstNodeId,
-        path_index: int,
+        referenced_declaration_id: AstNodeId,
+        reference_resolver: ReferenceResolver,
+        cu_hash: bytes,
+        file: Path,
     ):
         self._underlying_node = underlying_node
-        self._reference_resolver = init.reference_resolver
-        self._path_referenced_declaration_id = path_referenced_declaration_id
-        # zero-based index from the end of the path
-        self._path_index = path_index
-        self._referenced_declaration_id = None
-        self._cu_hash = init.cu.hash
-        self._file = init.file
+        self._reference_resolver = reference_resolver
+        self._referenced_declaration_id = referenced_declaration_id
+        self._cu_hash = cu_hash
+        self._file = file
         self._byte_location = byte_location
         self._name = name
 
         self._reference_resolver.register_post_process_callback(self._post_process)
 
     def _post_process(self, callback_params: CallbackParams):
-        from .source_unit import SourceUnit
-
-        referenced_declaration = self._reference_resolver.resolve_node(
-            self._path_referenced_declaration_id, self._cu_hash
-        )
-        for i in range(self._path_index):
-            assert referenced_declaration.parent is not None
-            referenced_declaration = referenced_declaration.parent
-        assert isinstance(referenced_declaration, (DeclarationAbc, SourceUnit))
-
-        node_path_order = self._reference_resolver.get_node_path_order(
-            AstNodeId(referenced_declaration.ast_node_id),
-            referenced_declaration.cu_hash,
-        )
-        this_cu_id = self._reference_resolver.get_ast_id_from_cu_node_path_order(
-            node_path_order, self._cu_hash
-        )
-        self._referenced_declaration_id = this_cu_id
-
+        referenced_declaration = self.referenced_declaration
         if isinstance(referenced_declaration, DeclarationAbc):
             referenced_declaration.register_reference(self)
             self._reference_resolver.register_destroy_callback(
                 self.file, partial(self._destroy, referenced_declaration)
             )
 
-    def _destroy(
-        self, referenced_declaration: Union[DeclarationAbc, SourceUnit]
-    ) -> None:
-        if isinstance(referenced_declaration, DeclarationAbc):
-            referenced_declaration.unregister_reference(self)
+    def _destroy(self, referenced_declaration: DeclarationAbc) -> None:
+        referenced_declaration.unregister_reference(self)
 
     @property
     def underlying_node(self) -> Union[IdentifierPath, UserDefinedTypeName]:
         """
         Returns:
             Underlying IR node (parent) of this identifier path part.
         """
@@ -180,30 +156,100 @@
         parent: SolidityAbc,
     ):
         super().__init__(init, identifier_path, parent)
         self._name = identifier_path.name
         self._referenced_declaration_id = identifier_path.referenced_declaration
         assert self._referenced_declaration_id >= 0
 
+        self._reference_resolver.register_post_process_callback(self._post_process)
+
+    def _post_process(self, callback_params: CallbackParams):
+        def find_referenced_source_unit(
+            searched_name: str, start_source_unit: SourceUnit
+        ) -> SourceUnit:
+            source_units_queue: Deque[SourceUnit] = deque([start_source_unit])
+            processed_source_units: Set[Path] = {start_source_unit.file}
+            referenced_declaration = None
+
+            while source_units_queue and referenced_declaration is None:
+                source_unit = source_units_queue.popleft()
+
+                for import_ in source_unit.imports:
+                    if import_.unit_alias == searched_name:
+                        referenced_declaration = callback_params.source_units[
+                            import_.imported_file
+                        ]
+                        break
+                    for symbol_alias in import_.symbol_aliases:
+                        if symbol_alias.local == searched_name:
+                            ref = symbol_alias.foreign.referenced_declaration
+                            assert isinstance(ref, SourceUnit)
+                            referenced_declaration = ref
+
+                    if referenced_declaration is not None:
+                        break
+
+                    if import_.imported_file not in processed_source_units:
+                        source_units_queue.append(
+                            callback_params.source_units[import_.imported_file]
+                        )
+                        processed_source_units.add(import_.imported_file)
+
+            assert referenced_declaration is not None
+            return referenced_declaration
+
+        from ..meta.source_unit import SourceUnit
+
         matches = list(IDENTIFIER_RE.finditer(self._source))
         groups_count = len(matches)
         assert groups_count > 0
 
         self._parts = IntervalTree()
-        for i, match in enumerate(matches):
+        start_source_unit = callback_params.source_units[self._file]
+
+        ref = self.referenced_declaration
+        refs = []
+        for _ in range(groups_count):
+            refs.append(ref)
+            if ref is not None:
+                ref = ref.parent
+
+        for match, ref in zip(matches, reversed(refs)):
             name = match.group(0).decode("utf-8")
+
+            if ref is None:
+                start_source_unit = find_referenced_source_unit(name, start_source_unit)
+                referenced_node = start_source_unit
+            elif isinstance(ref, (DeclarationAbc, SourceUnit)):
+                referenced_node = ref
+            else:
+                raise TypeError(
+                    f"Unexpected type of referenced declaration: {type(ref)}"
+                )
+
+            node_path_order = self._reference_resolver.get_node_path_order(
+                AstNodeId(referenced_node.ast_node_id),
+                referenced_node.cu_hash,
+            )
+            referenced_node_id = (
+                self._reference_resolver.get_ast_id_from_cu_node_path_order(
+                    node_path_order, self._cu_hash
+                )
+            )
+
             start = self.byte_location[0] + match.start()
             end = self.byte_location[0] + match.end()
             self._parts[start:end] = IdentifierPathPart(
                 self,
-                init,
                 (start, end),
                 name,
-                self._referenced_declaration_id,
-                groups_count - i - 1,
+                referenced_node_id,
+                self._reference_resolver,
+                self._cu_hash,
+                self._file,
             )
 
     @property
     def parent(
         self,
     ) -> Union[
         InheritanceSpecifier,
```

### Comparing `woke-3.3.0/woke/ast/ir/meta/import_directive.py` & `woke-3.4.0/woke/ast/ir/meta/import_directive.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             self._unit_alias = None
 
         for alias in import_directive.symbol_aliases:
             self._symbol_aliases.append(
                 SymbolAlias(Identifier(init, alias.foreign, self), alias.local)
             )
         self._reference_resolver.register_post_process_callback(
-            self._post_process, priority=-1
+            self._post_process, priority=-2
         )
 
     def __iter__(self) -> Iterator[IrAbc]:
         yield self
         for symbol_alias in self._symbol_aliases:
             yield from symbol_alias.foreign
 
@@ -144,14 +144,18 @@
 
                 for declaration in imported_source_unit.declarations_iter():
                     if declaration.canonical_name == searched_name:
                         referenced_declaration = declaration
                         break
 
                 for import_ in imported_source_unit.imports:
+                    if import_.unit_alias == searched_name:
+                        referenced_declaration = import_
+                        break
+
                     # handle the case when an imported symbol is an alias of another symbol
                     for alias in import_.symbol_aliases:
                         if alias.local == symbol_alias.foreign.name:
                             searched_name = alias.foreign.name
                     if import_.imported_file not in processed_source_units:
                         source_units_queue.append(
                             callback_params.source_units[import_.imported_file]
@@ -213,15 +217,15 @@
         node = self._reference_resolver.resolve_node(
             self._source_unit_id, self._cu_hash
         )
         assert isinstance(node, SourceUnit)
         return node
 
     @property
-    def symbol_aliases(self) -> Tuple[SymbolAlias]:
+    def symbol_aliases(self) -> Tuple[SymbolAlias, ...]:
         """
         Is only set in the case of `:::solidity import { SafeType as CustomSafeType } from "SafeLib.sol";` import directive type.
         Returns:
             Symbol aliases present in the import directive.
         """
         return tuple(self._symbol_aliases)
```

### Comparing `woke-3.3.0/woke/ast/ir/meta/inheritance_specifier.py` & `woke-3.4.0/woke/ast/ir/meta/inheritance_specifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                 owner = _owner;
             }
         }
 
         contract B is A(0x1234567890123456789012345678901234567890) {}
         ```
     """
+
     _ast_node: SolcInheritanceSpecifier
     _parent: ContractDefinition
 
     _base_name: Union[IdentifierPath, UserDefinedTypeName]
     _arguments: Optional[List[ExpressionAbc]]
 
     def __init__(
```

### Comparing `woke-3.3.0/woke/ast/ir/meta/modifier_invocation.py` & `woke-3.4.0/woke/ast/ir/meta/modifier_invocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Iterator, List, Optional, Union
 
+from ...enums import ModifierInvocationKind
 from ..expression.abc import ExpressionAbc
 from ..expression.identifier import Identifier
-from .identifier_path import IdentifierPath
 from ..reference_resolver import CallbackParams
-from ...enums import ModifierInvocationKind
+from .identifier_path import IdentifierPath
 
 if TYPE_CHECKING:
     from ..declaration.function_definition import FunctionDefinition
 
 from woke.ast.ir.abc import IrAbc, SolidityAbc
 from woke.ast.ir.utils import IrInitTuple
 from woke.ast.nodes import SolcIdentifier, SolcIdentifierPath, SolcModifierInvocation
@@ -31,14 +31,15 @@
         contract MyContract is ERC20, Initializable {
             constructor() ERC20("MyToken", "MTK") initializer {
                 // ...
             }
         }
         ```
     """
+
     _ast_node: SolcModifierInvocation
     _parent: FunctionDefinition
 
     _kind: Optional[ModifierInvocationKind]
     _modifier_name: Union[Identifier, IdentifierPath]
     _arguments: Optional[List[ExpressionAbc]]
```

### Comparing `woke-3.3.0/woke/ast/ir/meta/override_specifier.py` & `woke-3.4.0/woke/ast/ir/meta/override_specifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
             function transfer(address to, uint256 value) external override returns (bool) {
                 // ...
             }
         }
         ```
     """
+
     _ast_node: SolcOverrideSpecifier
     _parent: Union[FunctionDefinition, ModifierDefinition, VariableDeclaration]
 
     _overrides: List[Union[IdentifierPath, UserDefinedTypeName]]
 
     def __init__(
         self,
@@ -88,15 +89,15 @@
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
-    def overrides(self) -> Tuple[Union[IdentifierPath, UserDefinedTypeName]]:
+    def overrides(self) -> Tuple[Union[IdentifierPath, UserDefinedTypeName], ...]:
         """
         !!! note
             Is empty when there are no curly braces after the `:::solidity override` keyword.
         Returns:
             Tuple of IR nodes referencing the contract or interface whose declaration is being overridden.
         """
         return tuple(self._overrides)
```

### Comparing `woke-3.3.0/woke/ast/ir/meta/parameter_list.py` & `woke-3.4.0/woke/ast/ir/meta/parameter_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
                 } catch Error(string memory reason) {
                     // ...
                 }
             }
         }
         ```
     """
+
     _ast_node: SolcParameterList
     _parent: Union[
         ErrorDefinition,
         EventDefinition,
         FunctionDefinition,
         FunctionTypeName,
         ModifierDefinition,
@@ -106,14 +107,14 @@
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
-    def parameters(self) -> Tuple[VariableDeclaration]:
+    def parameters(self) -> Tuple[VariableDeclaration, ...]:
         """
         Can be empty.
         Returns:
             Variable declarations of the parameter list.
         """
         return tuple(self._parameters)
```

### Comparing `woke-3.3.0/woke/ast/ir/meta/pragma_directive.py` & `woke-3.4.0/woke/ast/ir/meta/pragma_directive.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
-    def literals(self) -> Tuple[str]:
+    def literals(self) -> Tuple[str, ...]:
         """
         !!! example
             `:::py ('solidity', '^', '0.8', '||', '0.7', '.1', '-', '0.7', '.6')` for the following pragma:
             ```solidity
             pragma solidity ^0.8 || 0.7.1 - 0.7.6;
             ```
         !!! example
```

### Comparing `woke-3.3.0/woke/ast/ir/meta/source_unit.py` & `woke-3.4.0/woke/ast/ir/meta/source_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,89 +173,89 @@
         """
         Returns:
             Source unit name of the file.
         """
         return self._source_unit_name
 
     @property
-    def pragmas(self) -> Tuple[PragmaDirective]:
+    def pragmas(self) -> Tuple[PragmaDirective, ...]:
         """
         Returns:
             Pragma directives present in the file.
         """
         return tuple(self._pragmas)
 
     @property
-    def imports(self) -> Tuple[ImportDirective]:
+    def imports(self) -> Tuple[ImportDirective, ...]:
         """
         Returns:
             Import directives present in the file.
         """
         return tuple(self._imports)
 
     @property
-    def declared_variables(self) -> Tuple[VariableDeclaration]:
+    def declared_variables(self) -> Tuple[VariableDeclaration, ...]:
         """
         Should only return constants.
         Returns:
             Top-level variable declarations present in the file.
         """
         return tuple(self._declared_variables)
 
     @property
-    def enums(self) -> Tuple[EnumDefinition]:
+    def enums(self) -> Tuple[EnumDefinition, ...]:
         """
         Returns:
             Top-level enum definitions present in the file.
         """
         return tuple(self._enums)
 
     @property
-    def functions(self) -> Tuple[FunctionDefinition]:
+    def functions(self) -> Tuple[FunctionDefinition, ...]:
         """
         Should only return [FunctionDefinitions][woke.ast.ir.declaration.function_definition.FunctionDefinition] of the [FunctionKind.FREE_FUNCTION][woke.ast.enums.FunctionKind.FREE_FUNCTION] kind.
         Returns:
             Top-level function definitions present in the file.
         """
         return tuple(self._functions)
 
     @property
-    def structs(self) -> Tuple[StructDefinition]:
+    def structs(self) -> Tuple[StructDefinition, ...]:
         """
         Returns:
             Top-level struct definitions present in the file.
         """
         return tuple(self._structs)
 
     @property
-    def errors(self) -> Tuple[ErrorDefinition]:
+    def errors(self) -> Tuple[ErrorDefinition, ...]:
         """
         Returns:
             Top-level error definitions present in the file.
         """
         return tuple(self._errors)
 
     @property
-    def user_defined_value_types(self) -> Tuple[UserDefinedValueTypeDefinition]:
+    def user_defined_value_types(self) -> Tuple[UserDefinedValueTypeDefinition, ...]:
         """
         Returns:
             Top-level user-defined value type definitions present in the file.
         """
         return tuple(self._user_defined_value_types)
 
     @property
-    def contracts(self) -> Tuple[ContractDefinition]:
+    def contracts(self) -> Tuple[ContractDefinition, ...]:
         """
         Returns:
             Contract definitions present in the file.
         """
         return tuple(self._contracts)
 
     @property
-    def using_for_directives(self) -> Tuple[UsingForDirective]:
+    def using_for_directives(self) -> Tuple[UsingForDirective, ...]:
         """
         Returns:
             Top-level using for directives present in the file.
         """
         return tuple(self._using_for_directives)
 
     def declarations_iter(self) -> Iterator[DeclarationAbc]:
```

### Comparing `woke-3.3.0/woke/ast/ir/meta/structured_documentation.py` & `woke-3.4.0/woke/ast/ir/meta/structured_documentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         contract Tree {
             function multiply(uint a) public pure returns(uint) {
                 return a * 7;
             }
         }
         ```
     """
+
     _ast_node: SolcStructuredDocumentation
     _parent: Union[
         ContractDefinition,
         ErrorDefinition,
         EventDefinition,
         FunctionDefinition,
         ModifierDefinition,
```

### Comparing `woke-3.3.0/woke/ast/ir/meta/try_catch_clause.py` & `woke-3.4.0/woke/ast/ir/meta/try_catch_clause.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/meta/using_for_directive.py` & `woke-3.4.0/woke/ast/ir/meta/using_for_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/reference_resolver.py` & `woke-3.4.0/woke/ast/ir/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/statement/abc.py` & `woke-3.4.0/woke/ast/ir/statement/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Iterator, Set, Tuple, Union, Optional
+from typing import TYPE_CHECKING, Iterator, Optional, Set, Tuple, Union
 
 from woke.ast.enums import ModifiesStateFlag
 from woke.ast.ir.abc import IrAbc, SolidityAbc
 from woke.ast.ir.utils import IrInitTuple
 from woke.ast.nodes import (
     SolcBlock,
     SolcBreak,
@@ -38,14 +38,15 @@
     from .while_statement import WhileStatement
 
 
 class StatementAbc(SolidityAbc, ABC):
     """
     Abstract base class for all Solidity statements.
     """
+
     _documentation: Optional[str]
 
     def __init__(
         self, init: IrInitTuple, statement: SolcStatementUnion, parent: SolidityAbc
     ):
         super().__init__(init, statement, parent)
         self._documentation = statement.documentation
```

### Comparing `woke-3.3.0/woke/ast/ir/statement/block.py` & `woke-3.4.0/woke/ast/ir/statement/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
-    def statements(self) -> Tuple[StatementAbc]:
+    def statements(self) -> Tuple[StatementAbc, ...]:
         """
         Can be empty.
         Returns:
             Statements in the block.
         """
         return tuple(self._statements)
```

### Comparing `woke-3.3.0/woke/ast/ir/statement/break_statement.py` & `woke-3.4.0/woke/ast/ir/statement/break_statement.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             for (uint i = 0; i < 10; i++) {
                 if (i == 5)
                     break;
             }
         }
         ```
     """
+
     _ast_node: SolcBreak
     _parent: Union[
         Block,
         DoWhileStatement,
         ForStatement,
         IfStatement,
         UncheckedBlock,
```

### Comparing `woke-3.3.0/woke/ast/ir/statement/continue_statement.py` & `woke-3.4.0/woke/ast/ir/statement/continue_statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             for (uint i = 0; i < 10; i++) {
                 if (i == 5)
                     continue;
             }
         }
         ```
     """
+
     _ast_node: SolcContinue
     _parent: Union[
         Block,
         DoWhileStatement,
         ForStatement,
         IfStatement,
         UncheckedBlock,
```

### Comparing `woke-3.3.0/woke/ast/ir/statement/do_while_statement.py` & `woke-3.4.0/woke/ast/ir/statement/do_while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/statement/emit_statement.py` & `woke-3.4.0/woke/ast/ir/statement/emit_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/statement/expression_statement.py` & `woke-3.4.0/woke/ast/ir/statement/expression_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/statement/for_statement.py` & `woke-3.4.0/woke/ast/ir/statement/for_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/statement/if_statement.py` & `woke-3.4.0/woke/ast/ir/statement/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/statement/inline_assembly.py` & `woke-3.4.0/woke/ast/ir/statement/inline_assembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
             ```
         Returns:
             Flags decorating the inline assembly block.
         """
         return frozenset(self._flags)
 
     @property
-    def external_references(self) -> Tuple[ExternalReference]:
+    def external_references(self) -> Tuple[ExternalReference, ...]:
         """
         Returns:
             External references in the inline assembly block.
         """
         return tuple(interval.data for interval in self._external_references)
 
     def external_reference_at(self, byte_offset: int) -> Optional[ExternalReference]:
```

### Comparing `woke-3.3.0/woke/ast/ir/statement/placeholder_statement.py` & `woke-3.4.0/woke/ast/ir/statement/placeholder_statement.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         ```solidity linenums="1"
         modifier foo() {
             require(msg.sender == owner, "Not owner");
             _;
         }
         ```
     """
+
     _ast_node: SolcPlaceholderStatement
     _parent: Union[Block, DoWhileStatement, ForStatement, IfStatement, WhileStatement]
 
     def __init__(
         self,
         init: IrInitTuple,
         placeholder_statement: SolcPlaceholderStatement,
```

### Comparing `woke-3.3.0/woke/ast/ir/statement/return_statement.py` & `woke-3.4.0/woke/ast/ir/statement/return_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/statement/revert_statement.py` & `woke-3.4.0/woke/ast/ir/statement/revert_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/statement/try_statement.py` & `woke-3.4.0/woke/ast/ir/statement/try_statement.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
-    def clauses(self) -> Tuple[TryCatchClause]:
+    def clauses(self) -> Tuple[TryCatchClause, ...]:
         """
         Returns:
             Try/catch clauses.
         """
         return tuple(self._clauses)
 
     @property
```

### Comparing `woke-3.3.0/woke/ast/ir/statement/unchecked_block.py` & `woke-3.4.0/woke/ast/ir/statement/unchecked_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
-    def statements(self) -> Tuple[StatementAbc]:
+    def statements(self) -> Tuple[StatementAbc, ...]:
         """
         Can be empty.
         Returns:
             Statements in the block.
         """
         return tuple(self._statements)
```

### Comparing `woke-3.3.0/woke/ast/ir/statement/variable_declaration_statement.py` & `woke-3.4.0/woke/ast/ir/statement/variable_declaration_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
-    def declarations(self) -> Tuple[Optional[VariableDeclaration]]:
+    def declarations(self) -> Tuple[Optional[VariableDeclaration], ...]:
         """
         !!! example
             Some declarations may be `None`, e.g. in the following code:
             ```solidity
             (bool success, ) = address(this).call{value: 1}("");
             ```
```

### Comparing `woke-3.3.0/woke/ast/ir/statement/while_statement.py` & `woke-3.4.0/woke/ast/ir/statement/while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/type_name/abc.py` & `woke-3.4.0/woke/ast/ir/type_name/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/type_name/array_type_name.py` & `woke-3.4.0/woke/ast/ir/type_name/array_type_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterator, Optional, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterator, Optional, Union
 
 from ...types import Array
 
 if TYPE_CHECKING:
     from ..declaration.variable_declaration import VariableDeclaration
     from ..expression.new_expression import NewExpression
     from ..meta.using_for_directive import UsingForDirective
@@ -55,39 +55,46 @@
 
             function foo() public pure {
                 address[] memory addresses = new address[](5);
             }
         }
         ```
     """
+
     _ast_node: SolcArrayTypeName
-    _parent: Union[VariableDeclaration, NewExpression, UsingForDirective, ArrayTypeName, Mapping]
+    _parent: Union[
+        VariableDeclaration, NewExpression, UsingForDirective, ArrayTypeName, Mapping
+    ]
 
     _base_type: TypeNameAbc
     _length: Optional[ExpressionAbc]
 
     def __init__(
         self, init: IrInitTuple, array_type_name: SolcArrayTypeName, parent: SolidityAbc
     ):
         super().__init__(init, array_type_name, parent)
         self._base_type = TypeNameAbc.from_ast(init, array_type_name.base_type, self)
         self._length = (
             ExpressionAbc.from_ast(init, array_type_name.length, self)
-            if array_type_name.length
+            if array_type_name.length is not None
             else None
         )
 
     def __iter__(self) -> Iterator[IrAbc]:
         yield self
         yield from self._base_type
         if self._length is not None:
             yield from self._length
 
     @property
-    def parent(self) -> Union[VariableDeclaration, NewExpression, UsingForDirective, ArrayTypeName, Mapping]:
+    def parent(
+        self,
+    ) -> Union[
+        VariableDeclaration, NewExpression, UsingForDirective, ArrayTypeName, Mapping
+    ]:
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
```

### Comparing `woke-3.3.0/woke/ast/ir/type_name/elementary_type_name.py` & `woke-3.4.0/woke/ast/ir/type_name/elementary_type_name.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 from __future__ import annotations
 
-from typing import Optional, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional, Union
 
-from ...types import Address, Bool, Int, UInt, String, Bytes, FixedBytes, Type, Fixed, UFixed
+from ...types import (
+    Address,
+    Bool,
+    Bytes,
+    Fixed,
+    FixedBytes,
+    Int,
+    String,
+    Type,
+    UFixed,
+    UInt,
+)
 
 if TYPE_CHECKING:
-    from ..declaration.user_defined_value_type_definition import UserDefinedValueTypeDefinition
+    from ..declaration.user_defined_value_type_definition import (
+        UserDefinedValueTypeDefinition,
+    )
     from ..declaration.variable_declaration import VariableDeclaration
-    from ..expression.elementary_type_name_expression import ElementaryTypeNameExpression
+    from ..expression.elementary_type_name_expression import (
+        ElementaryTypeNameExpression,
+    )
     from ..expression.new_expression import NewExpression
     from ..meta.using_for_directive import UsingForDirective
     from .array_type_name import ArrayTypeName
     from .mapping import Mapping
 
 from woke.ast.enums import StateMutability
 from woke.ast.ir.abc import IrAbc, SolidityAbc
@@ -61,16 +76,25 @@
 
             function foo() public pure {
                 bytes memory b = new bytes(10);
             }
         }
         ```
     """
+
     _ast_node: SolcElementaryTypeName
-    _parent: Union[VariableDeclaration, UserDefinedValueTypeDefinition, ElementaryTypeNameExpression, NewExpression, UsingForDirective, ArrayTypeName, Mapping]
+    _parent: Union[
+        VariableDeclaration,
+        UserDefinedValueTypeDefinition,
+        ElementaryTypeNameExpression,
+        NewExpression,
+        UsingForDirective,
+        ArrayTypeName,
+        Mapping,
+    ]
 
     _name: str
     _state_mutability: Optional[StateMutability]
 
     def __init__(
         self,
         init: IrInitTuple,
@@ -88,33 +112,53 @@
         # fix missing type descriptions in AST
         if self._type_descriptions.type_identifier is None and isinstance(
             parent, ElementaryTypeNameExpression
         ):
             self._type_descriptions = parent._type_descriptions
 
     @property
-    def parent(self) -> Union[VariableDeclaration, UserDefinedValueTypeDefinition, ElementaryTypeNameExpression, NewExpression, UsingForDirective, ArrayTypeName, Mapping]:
+    def parent(
+        self,
+    ) -> Union[
+        VariableDeclaration,
+        UserDefinedValueTypeDefinition,
+        ElementaryTypeNameExpression,
+        NewExpression,
+        UsingForDirective,
+        ArrayTypeName,
+        Mapping,
+    ]:
         """
         When the parent is a [NewExpression][woke.ast.ir.expression.new_expression.NewExpression], this can only be `bytes` or `string`.
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
-    def type(self) -> Union[Address, Bool, Int, UInt, Fixed, UFixed, String, Bytes, FixedBytes, Type]:
+    def type(
+        self,
+    ) -> Union[
+        Address, Bool, Int, UInt, Fixed, UFixed, String, Bytes, FixedBytes, Type
+    ]:
         """
         Returns either the generic [Type][woke.ast.types.Type] expression type (this is the case of a type conversion, for example `:::solidity address(0)`) or directly one of the elementary expression types.
         Returns:
             Type description.
         """
         t = super().type
-        if not isinstance(t, (Address, Bool, Int, UInt, Fixed, UFixed, String, Bytes, FixedBytes, Type)):
+        if not isinstance(
+            t,
+            (Address, Bool, Int, UInt, Fixed, UFixed, String, Bytes, FixedBytes, Type),
+        ):
             raise TypeError(f"Unexpected type {t} {self.source}")
-        assert isinstance(t, (Address, Bool, Int, UInt, Fixed, UFixed, String, Bytes, FixedBytes, Type))
+        assert isinstance(
+            t,
+            (Address, Bool, Int, UInt, Fixed, UFixed, String, Bytes, FixedBytes, Type),
+        )
         return t
 
     @property
     def name(self) -> str:
         """
         !!! example
             For example `uint256`, `bool`, `string`, `bytes1` or `address`.
```

### Comparing `woke-3.3.0/woke/ast/ir/type_name/function_type_name.py` & `woke-3.4.0/woke/ast/ir/type_name/function_type_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterator, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterator, Union
 
 from ...types import Function
 
 if TYPE_CHECKING:
     from ..declaration.variable_declaration import VariableDeclaration
     from ..meta.using_for_directive import UsingForDirective
     from .array_type_name import ArrayTypeName
@@ -46,14 +46,15 @@
             function foo(uint a) public returns(uint){
                 x = foo;
                 y.push(foo);
             }
         }
         ```
     """
+
     _ast_node: SolcFunctionTypeName
     _parent: Union[VariableDeclaration, UsingForDirective, ArrayTypeName, Mapping]
 
     _parameter_types: ParameterList
     _return_parameter_types: ParameterList
     _state_mutability: StateMutability
     _visibility: Visibility
@@ -76,15 +77,17 @@
 
     def __iter__(self) -> Iterator[IrAbc]:
         yield self
         yield from self._parameter_types
         yield from self._return_parameter_types
 
     @property
-    def parent(self) -> Union[VariableDeclaration, UsingForDirective, ArrayTypeName, Mapping]:
+    def parent(
+        self,
+    ) -> Union[VariableDeclaration, UsingForDirective, ArrayTypeName, Mapping]:
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
```

### Comparing `woke-3.3.0/woke/ast/ir/type_name/mapping.py` & `woke-3.4.0/woke/ast/ir/type_name/mapping.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterator, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterator, Union
 
 from .elementary_type_name import ElementaryTypeName
 from .user_defined_type_name import UserDefinedTypeName
 
 if TYPE_CHECKING:
     from ..declaration.variable_declaration import VariableDeclaration
     from ..meta.using_for_directive import UsingForDirective
@@ -43,14 +43,15 @@
 
         contract C {
             mapping(address => mapping(address => uint)) public allowances;
             mapping(address => uint)[2] public balances;
         }
         ```
     """
+
     _ast_node: SolcMapping
     _parent: Union[VariableDeclaration, UsingForDirective, ArrayTypeName, Mapping]
 
     _key_type: Union[ElementaryTypeName, UserDefinedTypeName]
     _value_type: TypeNameAbc
 
     def __init__(self, init: IrInitTuple, mapping: SolcMapping, parent: SolidityAbc):
@@ -62,15 +63,17 @@
 
     def __iter__(self) -> Iterator[IrAbc]:
         yield self
         yield from self._key_type
         yield from self._value_type
 
     @property
-    def parent(self) -> Union[VariableDeclaration, UsingForDirective, ArrayTypeName, Mapping]:
+    def parent(
+        self,
+    ) -> Union[VariableDeclaration, UsingForDirective, ArrayTypeName, Mapping]:
         """
         Returns:
             Parent IR node.
         """
         return self._parent
 
     @property
```

### Comparing `woke-3.3.0/woke/ast/ir/utils/init_tuple.py` & `woke-3.4.0/woke/ast/ir/utils/init_tuple.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/yul/__init__.py` & `woke-3.4.0/woke/ast/ir/yul/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/yul/abc.py` & `woke-3.4.0/woke/ast/ir/yul/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ..abc import IrAbc
 
 
 class YulAbc(IrAbc, ABC):
     """
     Abstract base class for all Yul IR nodes.
     """
+
     _ast_node: YulNode
 
     def __iter__(self) -> Iterator[YulAbc]:
         yield self
 
     @property
     def ast_node(self) -> YulNode:
@@ -28,8 +29,9 @@
         return set()  # TODO
 
 
 class YulStatementAbc(YulAbc, ABC):
     """
     Abstract base class for all Yul IR statements.
     """
+
     pass
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/assignment.py` & `woke-3.4.0/woke/ast/ir/yul/assignment.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     from .block import Block
 
 
 class Assignment(YulStatementAbc):
     """
     TBD
     """
+
     _parent: Block
     _value: Union[FunctionCall, Identifier, Literal]
     _variable_names: List[Identifier]
 
     def __init__(self, init: IrInitTuple, assignment: YulAssignment, parent: YulAbc):
         super().__init__(init, assignment, parent)
         if isinstance(assignment.value, YulFunctionCall):
@@ -48,9 +49,9 @@
         return self._parent
 
     @property
     def value(self) -> Union[FunctionCall, Identifier, Literal]:
         return self._value
 
     @property
-    def variable_names(self) -> Tuple[Identifier]:
+    def variable_names(self) -> Tuple[Identifier, ...]:
         return tuple(self._variable_names)
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/block.py` & `woke-3.4.0/woke/ast/ir/yul/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     from .variable_declaration import VariableDeclaration
 
 
 class Block(YulStatementAbc):
     """
     TBD
     """
+
     _parent: Union[InlineAssembly, Block, ForLoop, FunctionDefinition, If, Case]
     _statements: List[
         Union[
             Assignment,
             "Block",
             Break,
             Continue,
@@ -121,10 +122,11 @@
             ExpressionStatement,
             Leave,
             ForLoop,
             FunctionDefinition,
             If,
             Switch,
             VariableDeclaration,
-        ]
+        ],
+        ...,
     ]:
         return tuple(self._statements)
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/case_statement.py` & `woke-3.4.0/woke/ast/ir/yul/case_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     from .switch import Switch
 
 
 class Case(YulAbc):
     """
     TBD
     """
+
     _parent: Switch
     _body: Block
     _value: Union[typing_extensions.Literal["default"], Literal]
 
     def __init__(self, init: IrInitTuple, case_: YulCase, parent: YulAbc):
         super().__init__(init, case_, parent)
         self._body = Block(init, case_.body, self)
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/expression_statement.py` & `woke-3.4.0/woke/ast/ir/yul/expression_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     from .block import Block
 
 
 class ExpressionStatement(YulStatementAbc):
     """
     TBD
     """
+
     _parent: Block
     _expression: Union[FunctionCall, Identifier, Literal]
 
     def __init__(
         self,
         init: IrInitTuple,
         expression_statement: YulExpressionStatement,
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/for_loop.py` & `woke-3.4.0/woke/ast/ir/yul/for_loop.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/yul/function_call.py` & `woke-3.4.0/woke/ast/ir/yul/function_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     from .variable_declaration import VariableDeclaration
 
 
 class FunctionCall(YulAbc):
     """
     TBD
     """
+
     _parent: Union[
         Assignment,
         ExpressionStatement,
         ForLoop,
         If,
         Switch,
         VariableDeclaration,
@@ -67,13 +68,13 @@
         Switch,
         VariableDeclaration,
         FunctionCall,
     ]:
         return self._parent
 
     @property
-    def arguments(self) -> Tuple[Union["FunctionCall", Identifier, Literal]]:
+    def arguments(self) -> Tuple[Union["FunctionCall", Identifier, Literal], ...]:
         return tuple(self._arguments)
 
     @property
     def function_name(self) -> Identifier:
         return self._function_name
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/function_definition.py` & `woke-3.4.0/woke/ast/ir/yul/function_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,17 +63,17 @@
         return self._body
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def parameters(self) -> Optional[Tuple[TypedName]]:
+    def parameters(self) -> Optional[Tuple[TypedName, ...]]:
         if self._parameters is None:
             return None
         return tuple(self._parameters)
 
     @property
-    def return_variables(self) -> Optional[Tuple[TypedName]]:
+    def return_variables(self) -> Optional[Tuple[TypedName, ...]]:
         if self._return_variables is None:
             return None
         return tuple(self._return_variables)
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/identifier.py` & `woke-3.4.0/woke/ast/ir/yul/identifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/yul/if_statement.py` & `woke-3.4.0/woke/ast/ir/yul/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/ast/ir/yul/literal.py` & `woke-3.4.0/woke/ast/ir/yul/literal.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     from .variable_declaration import VariableDeclaration
 
 
 class Literal(YulAbc):
     """
     TBD
     """
+
     _parent: Union[
         Assignment,
         ExpressionStatement,
         ForLoop,
         If,
         Switch,
         VariableDeclaration,
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/switch.py` & `woke-3.4.0/woke/ast/ir/yul/switch.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     from .block import Block
 
 
 class Switch(YulStatementAbc):
     """
     TBD
     """
+
     _parent: Block
     _cases: List[Case]
     _expression: Union[FunctionCall, Identifier, Literal]
 
     def __init__(self, init: IrInitTuple, switch: YulSwitch, parent: YulAbc):
         super().__init__(init, switch, parent)
         if isinstance(switch.expression, YulFunctionCall):
@@ -41,13 +42,13 @@
             yield from case_
 
     @property
     def parent(self) -> Block:
         return self._parent
 
     @property
-    def cases(self) -> Tuple[Case]:
+    def cases(self) -> Tuple[Case, ...]:
         return tuple(self._cases)
 
     @property
     def expression(self) -> Union[FunctionCall, Identifier, Literal]:
         return self._expression
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/typed_name.py` & `woke-3.4.0/woke/ast/ir/yul/typed_name.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     from .variable_declaration import VariableDeclaration
 
 
 class TypedName(YulAbc):
     """
     TBD
     """
+
     _parent: Union[FunctionDefinition, VariableDeclaration]
     _name: str
     _type: str
 
     def __init__(self, init: IrInitTuple, typed_name: YulTypedName, parent: YulAbc):
         super().__init__(init, typed_name, parent)
         self._name = typed_name.name
```

### Comparing `woke-3.3.0/woke/ast/ir/yul/variable_declaration.py` & `woke-3.4.0/woke/ast/ir/yul/variable_declaration.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     from .block import Block
 
 
 class VariableDeclaration(YulStatementAbc):
     """
     TBD
     """
+
     _parent: Block
     _variables: List[TypedName]
     _value: Optional[Union[FunctionCall, Identifier, Literal]]
 
     def __init__(
         self,
         init: IrInitTuple,
@@ -52,13 +53,13 @@
             yield from self._value
 
     @property
     def parent(self) -> Block:
         return self._parent
 
     @property
-    def variables(self) -> Tuple[TypedName]:
+    def variables(self) -> Tuple[TypedName, ...]:
         return tuple(self._variables)
 
     @property
     def value(self) -> Optional[Union[FunctionCall, Identifier, Literal]]:
         return self._value
```

### Comparing `woke-3.3.0/woke/ast/nodes.py` & `woke-3.4.0/woke/ast/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,14 +415,15 @@
     node_type: Literal["EnumDefinition"] = Field(alias="nodeType")
     # required
     name: StrictStr
     canonical_name: StrictStr
     members: List["SolcEnumValue"]
     # optional
     name_location: Optional[Src]  # new in 0.8.2
+    documentation: Optional["SolcStructuredDocumentation"]  # new in 0.8.20
 
 
 class SolcFunctionDefinition(SolcNode):
     # override alias
     node_type: Literal["FunctionDefinition"] = Field(alias="nodeType")
     # required
     name: StrictStr
@@ -451,14 +452,15 @@
     name: StrictStr
     canonical_name: StrictStr
     members: List["SolcVariableDeclaration"]
     scope: AstNodeId
     visibility: Visibility
     # optional
     name_location: Optional[Src]  # new in 0.8.2
+    documentation: Optional["SolcStructuredDocumentation"]  # new in 0.8.20
 
 
 # new in 0.8.4
 class SolcErrorDefinition(SolcNode):
     # override alias
     node_type: Literal["ErrorDefinition"] = Field(alias="nodeType")
     # required
@@ -502,14 +504,18 @@
         StrictStr
     ]  # should be present but because of a bug it is exported in >=0.8.9
     fully_implemented: Optional[
         StrictBool
     ]  # missing when a file that imports the contract cannot be compiled
     documentation: Optional[Union["SolcStructuredDocumentation", str]]
     used_errors: Optional[List[AstNodeId]]  # new in 0.8.4
+    used_events: Optional[List[AstNodeId]]  # new in 0.8.20
+    internal_function_ids: Optional[Dict[int, StrictInt]] = Field(
+        alias="internalFunctionIDs"
+    )
 
 
 class SolcEventDefinition(SolcNode):
     # override alias
     node_type: Literal["EventDefinition"] = Field(alias="nodeType")
     # required
     name: StrictStr
```

### Comparing `woke-3.3.0/woke/ast/types.py` & `woke-3.4.0/woke/ast/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,17 +769,20 @@
         self.__components = _parse_list(type_identifier, reference_resolver, cu_hash)
 
     def abi_type(self) -> str:
         if any(component is None for component in self.__components):
             raise NotImplementedError
         return (
             "("
-            + ",".join(component.abi_type() for component in self.__components)
+            + ",".join(
+                component.abi_type()  # pyright: ignore reportOptionalMemberAccess
+                for component in self.__components
+            )
             + ")"
-        )  # pyright: reportOptionalMemberAccess=false
+        )
 
     @property
     def components(self) -> typ.Tuple[typ.Optional[TypeAbc], ...]:
         """
         A component type can be `None` in the case of a tuple with a missing component.
         !!! example
             In the following example, the `(success, )` expression is of the [Tuple][woke.ast.types.Tuple] type with the components of the type [Bool][woke.ast.types.Bool] and `None`.
```

### Comparing `woke-3.3.0/woke/cli/__main__.py` & `woke-3.4.0/woke/cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 from .lsp import run_lsp
 from .run import run_run
 from .svm import run_svm
 from .test import run_test
 
 if platform.system() != "Windows":
     try:
-        from asyncio import (  # pyright: reportGeneralTypeIssues=false
-            ThreadedChildWatcher,
+        from asyncio import (
+            ThreadedChildWatcher,  # pyright: ignore reportGeneralTypeIssues
         )
     except ImportError:
         from woke.utils.threaded_child_watcher import ThreadedChildWatcher
 
 
 @click.group()
 @click.option("--debug/--no-debug", default=False)
```

### Comparing `woke-3.3.0/woke/cli/accounts.py` & `woke-3.4.0/woke/cli/accounts.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/cli/compile.py` & `woke-3.4.0/woke/cli/compile.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/cli/detect.py` & `woke-3.4.0/woke/cli/detect.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/cli/fuzz.py` & `woke-3.4.0/woke/cli/fuzz.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/cli/init.py` & `woke-3.4.0/woke/cli/init.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/cli/lsp.py` & `woke-3.4.0/woke/cli/lsp.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/cli/run.py` & `woke-3.4.0/woke/cli/run.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/cli/svm.py` & `woke-3.4.0/woke/cli/svm.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/cli/test.py` & `woke-3.4.0/woke/cli/test.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/compiler/build_data_model.py` & `woke-3.4.0/woke/compiler/build_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/compiler/compilation_unit.py` & `woke-3.4.0/woke/compiler/compilation_unit.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import networkx as nx
 from Crypto.Hash import BLAKE2b
 
 from woke.compiler.source_path_resolver import SourcePathResolver
 from woke.config import WokeConfig
 from woke.core.solidity_version import SolidityVersionRanges
 
+# pyright: reportGeneralTypeIssues=false
+
 
 class CompilationUnit:
     __unit_graph: nx.DiGraph
     __version_ranges: SolidityVersionRanges
     __hash: bytes
     __paths_to_source_unit_names: DefaultDict[Path, Set[str]]
```

### Comparing `woke-3.3.0/woke/compiler/compiler.py` & `woke-3.4.0/woke/compiler/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,16 @@
     SolcOutputError,
     SolcOutputErrorSeverityEnum,
     SolcOutputSelectionEnum,
 )
 from .source_path_resolver import SourcePathResolver
 from .source_unit_name_resolver import SourceUnitNameResolver
 
+# pyright: reportGeneralTypeIssues=false
+
 logger = logging.getLogger(__name__)
 
 
 class CompilationFileSystemEventHandler(FileSystemEventHandler):
     _config: WokeConfig
     _config_path: Path
     _compiler: SolidityCompiler
@@ -847,17 +849,15 @@
             else nullcontext()
         )
         start = time.perf_counter()
 
         with ctx_manager:
             # wait for compilation of all compilation units
             try:
-                ret: Tuple[SolcOutput, ...] = await asyncio.gather(
-                    *tasks
-                )  # pyright: ignore[reportGeneralTypeIssues]
+                ret: Tuple[SolcOutput, ...] = await asyncio.gather(*tasks)
             except Exception:
                 for task in tasks:
                     task.cancel()
                 raise
 
         end = time.perf_counter()
         if console is not None:
```

### Comparing `woke-3.3.0/woke/compiler/solc_frontend/input_data_model.py` & `woke-3.4.0/woke/compiler/solc_frontend/input_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/compiler/solc_frontend/output_data_model.py` & `woke-3.4.0/woke/compiler/solc_frontend/output_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/compiler/solc_frontend/solc_runner.py` & `woke-3.4.0/woke/compiler/solc_frontend/solc_runner.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/compiler/source_path_resolver.py` & `woke-3.4.0/woke/compiler/source_path_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/compiler/source_unit_name_resolver.py` & `woke-3.4.0/woke/compiler/source_unit_name_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
 
     __config: WokeConfig
 
     def __init__(self, woke_config: WokeConfig):
         self.__config = woke_config
 
-    def __apply_remapping(self, parent_source_unit: str, source_unit_name: str) -> str:
+    def apply_remapping(self, parent_source_unit: str, source_unit_name: str) -> str:
         """
         Try to apply a remapping and return a source unit name. Up to one remapping can be applied to a single import.
         It is the longest one. In case of multiple remappings with the same length, the one specified last wins.
         """
         matching_remappings: List[SolcRemapping] = []
         for remapping in self.__config.compiler.solc.remappings:
             context, prefix, target = remapping
@@ -48,15 +48,15 @@
             str(target_remapping.prefix), target_remapping.target or "", 1
         )
 
     def __resolve_direct_import(self, parent_source_unit: str, import_str: str) -> str:
         """
         Return a source unit name of a direct import in the file with given source unit name.
         """
-        return self.__apply_remapping(parent_source_unit, import_str)
+        return self.apply_remapping(parent_source_unit, import_str)
 
     def __resolve_relative_import(
         self, parent_source_unit: str, import_str: str
     ) -> str:
         """
         Return a source unit name of a relative import in the file with given source unit name.
         """
@@ -95,15 +95,15 @@
 
         if len(parent_parts) > 0:
             source_unit_name = (
                 "/".join(parent_parts) + "/" + "/".join(normalized_import_parts)
             )
         else:
             source_unit_name = "/".join(normalized_import_parts)
-        return self.__apply_remapping(parent_source_unit, source_unit_name)
+        return self.apply_remapping(parent_source_unit, source_unit_name)
 
     def resolve_import(self, parent_source_unit: str, import_str: str) -> str:
         """
         Resolve a source unit name of an import in the file with given source unit name.
         """
         if import_str.startswith((".", "..")):
             return self.__resolve_relative_import(parent_source_unit, import_str)
```

### Comparing `woke-3.3.0/woke/config/__init__.py` & `woke-3.4.0/woke/config/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/config/data_model.py` & `woke-3.4.0/woke/config/data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,17 @@
     )
     linearized_inheritance_graph: LinearizedInheritanceGraphConfig = Field(
         default_factory=LinearizedInheritanceGraphConfig
     )
 
 
 class AnvilConfig(WokeConfigModel):
-    cmd_args: str = "--prune-history 100 --steps-tracing --silent"
+    cmd_args: str = (
+        "--prune-history 100 --transaction-block-keeper 10 --steps-tracing --silent"
+    )
 
 
 class GanacheConfig(WokeConfigModel):
     cmd_args: str = "-k istanbul -q"
 
 
 class HardhatConfig(WokeConfigModel):
```

### Comparing `woke-3.3.0/woke/config/woke_config.py` & `woke-3.4.0/woke/config/woke_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,17 @@
         config_raw_copy = deepcopy(self.__config_raw)
 
         self.__load_file(None, path.resolve(), config_raw_copy, subconfigs_graph)
 
         config = TopLevelConfig.parse_obj(config_raw_copy)
         self.__config_raw = config_raw_copy
         self.__config = config
-        self.__loaded_files.update(subconfigs_graph.nodes)
+        self.__loaded_files.update(
+            subconfigs_graph.nodes  # pyright: ignore reportGeneralTypeIssues
+        )
 
     @property
     def loaded_files(self) -> FrozenSet[Path]:
         """
         Return frozenset of all loaded config file paths, including files that were loaded using the `subconfigs` config key.
         """
         return frozenset(self.__loaded_files)
@@ -321,15 +323,15 @@
 
     @property
     def min_solidity_version(self) -> SolidityVersion:
         return SolidityVersion.fromstring("0.6.2")
 
     @property
     def max_solidity_version(self) -> SolidityVersion:
-        return SolidityVersion.fromstring("0.8.19")
+        return SolidityVersion.fromstring("0.8.20")
 
     @property
     def detectors(self) -> DetectorsConfig:
         return self.__config.detectors
 
     @property
     def api_keys(self) -> Dict[str, str]:
```

### Comparing `woke-3.3.0/woke/contracts/woke/console.sol` & `woke-3.4.0/woke/contracts/woke/console.sol`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/core/solidity_version.py` & `woke-3.4.0/woke/core/solidity_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
 
 class SolidityVersionRanges:
     """
     Helper class implementing intersection on List[SolidityVersionRange].
     """
 
-    __version_ranges: Tuple[SolidityVersionRange]
+    __version_ranges: Tuple[SolidityVersionRange, ...]
 
     def __init__(self, version_ranges: Iterable[SolidityVersionRange]):
         self.__version_ranges = tuple(version_ranges)
 
     def __and__(self, other):
         if not isinstance(other, SolidityVersionRanges):
             return NotImplemented
```

### Comparing `woke-3.3.0/woke/deployment/__init__.py` & `woke-3.4.0/woke/deployment/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Panic,
     PanicCodeEnum,
     TransactionAbc,
     TransactionRevertedError,
     UnknownTransactionRevertedError,
     may_revert,
     must_revert,
+    on_revert,
 )
 from woke.development.utils import (
     get_create2_address_from_code,
     get_create2_address_from_hash,
     get_create_address,
     keccak256,
 )
```

### Comparing `woke-3.3.0/woke/deployment/core.py` & `woke-3.4.0/woke/deployment/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,18 +386,16 @@
                     completed=(latest_block_number - tx.block_number + 1),
                 )
             while latest_block_number - tx.block_number < confirmations - 1:
                 time.sleep(1)
                 latest_block_number = self.chain_interface.get_block_number()
                 if progress is not None:
                     progress.update(
-                        task_id,
-                        completed=(
-                            latest_block_number - tx.block_number + 1
-                        ),  # pyright: reportUnboundVariable=false
+                        task_id,  # pyright: ignore reportUnboundVariable
+                        completed=(latest_block_number - tx.block_number + 1),
                     )
 
     def _confirm_transaction(self, tx: TxParams) -> None:
         config = get_config()
         if config.deployment.silent:
             return
         pprint(tx, console=console, max_string=200)
```

### Comparing `woke-3.3.0/woke/development/blocks.py` & `woke-3.4.0/woke/development/blocks.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/call_trace.py` & `woke-3.4.0/woke/development/call_trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import importlib
 import reprlib
 from collections import ChainMap
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, cast
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple, cast
 
 import eth_abi
+import eth_abi.abi
 import eth_abi.exceptions
 import eth_utils
 from rich.console import Console
 from rich.highlighter import ReprHighlighter
 from rich.text import Text
 from rich.tree import Tree
 
@@ -147,27 +148,27 @@
     def __init__(
         self,
         contract: Optional[Contract],
         contract_name: Optional[str],
         function_name: Optional[str],
         selector: Optional[bytes],
         address: Optional[Address],
-        arguments: Optional[List],
+        arguments: Optional[Iterable],
         value: int,
         kind: CallTraceKind,
         depth: int,
         chain: Chain,
         function_is_special: bool = False,
     ):
         self._contract = contract
         self._contract_name = contract_name
         self._function_name = function_name
         self._selector = selector
         self._address = address
-        self._arguments = arguments
+        self._arguments = list(arguments) if arguments is not None else None
         self._value = Wei(value)
         self._kind = kind
         self._depth = depth
         self._chain = chain
         self._function_is_special = function_is_special
         self._status = True
         self._subtraces = []
@@ -242,16 +243,18 @@
             Text.from_markup(
                 f" {'[green]✓[/green]' if self.status else '[red]✗[/red]'}"
             )
         )
 
         if self.kind != CallTraceKind.CALL:
             ret.append_text(
-                Text.from_markup(f" [yellow]\[{self.kind}][/yellow]")
-            )  # pyright: reportInvalidStringEscapeSequence=false
+                Text.from_markup(
+                    f" [yellow]\[{self.kind}][/yellow]"  # pyright: ignore reportInvalidStringEscapeSequence
+                )
+            )
 
         return ret
 
     @property
     def subtraces(self) -> Tuple[CallTrace, ...]:
         return tuple(self._subtraces)
 
@@ -311,15 +314,17 @@
         fqn_overrides: ChainMap[Address, Optional[str]] = ChainMap()
 
         # process fqn_overrides for all txs before this one in the same block
         for i in range(tx.tx_index):
             tx_before = tx.block.txs[i]
             tx_before._fetch_debug_trace_transaction()
             process_debug_trace_for_fqn_overrides(
-                tx_before, tx_before._debug_trace_transaction, fqn_overrides
+                tx_before,
+                tx_before._debug_trace_transaction,  # pyright: ignore reportGeneralTypeIssues
+                fqn_overrides,
             )
 
         assert len(fqn_overrides.maps) == 1
 
         if tx.to is None:
             try:
                 origin_fqn, _ = get_fqn_from_creation_code(tx.data)
@@ -417,15 +422,15 @@
                         for arg in fix_library_abi(fn_abi["inputs"])
                     ]
                     try:
                         args = list(
                             eth_abi.abi.decode(
                                 output_types, tx_params["data"][constructor_offset:]
                             )
-                        )  # pyright: reportGeneralTypeIssues=false
+                        )
                     except eth_abi.exceptions.DecodingError:
                         args = None
                 root_trace = CallTrace(
                     obj,
                     contract_name,
                     "constructor",
                     None,
@@ -496,15 +501,15 @@
                 output_types = [
                     eth_utils.abi.collapse_if_tuple(cast(Dict[str, Any], arg))
                     for arg in fix_library_abi(fn_abi["inputs"])
                 ]
                 try:
                     decoded_data = list(
                         eth_abi.abi.decode(output_types, tx_params["data"][4:])
-                    )  # pyright: reportGeneralTypeIssues=false
+                    )
                 except eth_abi.exceptions.DecodingError:
                     decoded_data = None
                 root_trace = CallTrace(
                     obj,
                     contract_name,
                     fn_abi["name"],
                     tx_params["data"][:4],
@@ -582,15 +587,15 @@
                                     cast(Dict[str, Any], arg)
                                 )
                                 for arg in fix_library_abi(fn_abi)
                             ]
                             try:
                                 arguments = list(
                                     eth_abi.abi.decode(output_types, data[4:])
-                                )  # pyright: reportGeneralTypeIssues=false
+                                )
                             except eth_abi.exceptions.DecodingError:
                                 arguments = None
                         else:
                             arguments = [data]
 
                         call_trace = CallTrace(
                             None,
@@ -654,15 +659,15 @@
                                     cast(Dict[str, Any], arg)
                                 )
                                 for arg in fix_library_abi(fn_abi["inputs"])
                             ]
                             try:
                                 arguments = list(
                                     eth_abi.abi.decode(output_types, data[4:])
-                                )  # pyright: reportGeneralTypeIssues=false
+                                )
                             except eth_abi.exceptions.DecodingError:
                                 arguments = None
                             fn_name = fn_abi["name"]
                             is_special = False
                         elif "fallback" in contract_abi and (
                             value == 0
                             or contract_abi["fallback"]["stateMutability"] == "payable"
@@ -734,15 +739,15 @@
                 if current_trace.kind in {CallTraceKind.CREATE, CallTraceKind.CREATE2}:
                     try:
                         address = Address(
                             int(trace["structLogs"][i + 1]["stack"][-1], 16)
                         )
                         if address != Address(0):
                             current_trace._address = address
-                            fqn_overrides.maps[0][current_trace.address] = contracts[-1]
+                            fqn_overrides.maps[0][address] = contracts[-1]
                     except IndexError:
                         pass
 
                 current_trace._status = status
                 current_trace = current_trace._parent
 
                 contracts.pop()
@@ -772,15 +777,15 @@
                             for arg in fix_library_abi(fn_abi["inputs"])
                         ]
                         try:
                             args = list(
                                 eth_abi.abi.decode(
                                     output_types, creation_code[constructor_offset:]
                                 )
-                            )  # pyright: reportGeneralTypeIssues=false
+                            )
                         except eth_abi.exceptions.DecodingError:
                             args = None
                 except ValueError:
                     fqn = None
                     obj = None
                     contract_name = None
                     args = []
```

### Comparing `woke-3.3.0/woke/development/chain_interfaces.py` & `woke-3.4.0/woke/development/chain_interfaces.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/constants.py` & `woke-3.4.0/woke/development/constants.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/core.py` & `woke-3.4.0/woke/development/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import collections
 import dataclasses
 import functools
 import importlib
 import inspect
 import json
 import math
 import re
@@ -26,19 +25,19 @@
     List,
     Optional,
     Set,
     Tuple,
     Type,
     Union,
     cast,
-    overload,
 )
 from urllib.error import HTTPError
 
 import eth_abi
+import eth_abi.abi
 import eth_abi.packed
 import eth_account
 import eth_account.messages
 import eth_utils
 from Crypto.Hash import BLAKE2b, keccak
 from typing_extensions import (
     Annotated,
@@ -148,25 +147,19 @@
                 ret.append(str(arg.address))
             else:
                 ret.append(arg)
         return ret
 
     @classmethod
     def encode(cls, types: Iterable, arguments: Iterable) -> bytes:
-        return eth_abi.encode(  # pyright: ignore[reportPrivateImportUsage]
-            types, cls._normalize_arguments(arguments)
-        )
+        return eth_abi.abi.encode(types, cls._normalize_arguments(arguments))
 
     @classmethod
     def encode_packed(cls, types: Iterable, arguments: Iterable) -> bytes:
-        return (
-            eth_abi.packed.encode_packed(  # pyright: ignore[reportPrivateImportUsage]
-                types, cls._normalize_arguments(arguments)
-            )
-        )
+        return eth_abi.packed.encode_packed(types, cls._normalize_arguments(arguments))
 
     @classmethod
     def encode_with_selector(
         cls, selector: bytes, types: Iterable, arguments: Iterable
     ) -> bytes:
         return selector + cls.encode(types, arguments)
 
@@ -201,26 +194,28 @@
                     return c
             return getattr(
                 meth, "__objclass__", None
             )  # handle special descriptor objects
 
         selector = func.selector
         contract = get_class_that_defined_method(func)
-        assert selector in contract._abi  # pyright: reportOptionalMemberAccess=false
+        assert selector in contract._abi  # pyright: ignore reportGeneralTypeIssues
         types = [
             eth_utils.abi.collapse_if_tuple(cast(Dict[str, Any], arg))
             for arg in fix_library_abi(
-                contract._abi[selector]["inputs"]
-            )  # pyright: reportOptionalMemberAccess=false
+                contract._abi[selector][  # pyright: ignore reportGeneralTypeIssues
+                    "inputs"
+                ]
+            )
         ]
         return cls.encode_with_selector(selector, types, arguments)
 
     @classmethod
     def decode(cls, types: Iterable, data: bytes) -> Any:
-        return eth_abi.decode(types, data)  # pyright: ignore[reportPrivateImportUsage]
+        return eth_abi.abi.decode(types, data)
 
 
 class Wei(int):
     def to_ether(self) -> float:
         return self / 10**18
 
     def to_gwei(self) -> float:
@@ -233,30 +228,29 @@
     @classmethod
     def from_gwei(cls, value: Union[int, float]) -> Wei:
         return cls(int(value * 10**9))
 
     @classmethod
     def from_str(cls, value: str) -> Wei:
         count, unit = value.split()
-        return cls(eth_utils.to_wei(float(count), unit))
+        return cls(eth_utils.currency.to_wei(float(count), unit))
 
 
 @functools.total_ordering
 class Address:
     ZERO: Address
+    _private_key: Optional[bytes] = None
 
     def __init__(self, address: Union[str, int]) -> None:
         if isinstance(address, int):
             self._address = format(address, "#042x")
         elif isinstance(address, str):
             if not address.startswith(("0x", "0X")):
                 address = "0x" + address
-            if not eth_utils.is_address(
-                address
-            ):  # pyright: reportPrivateImportUsage=false
+            if not eth_utils.address.is_address(address):
                 raise ValueError(f"{address} is not a valid address")
             self._address = address
         else:
             raise TypeError("Expected a string or int")
 
     def __str__(self) -> str:
         return self._address
@@ -290,14 +284,74 @@
 
     def __hash__(self) -> int:
         return hash(self._address.lower())
 
     def __bytes__(self) -> bytes:
         return bytes.fromhex(self._address[2:])
 
+    @classmethod
+    def from_key(cls, private_key: Union[str, int, bytes]) -> Address:
+        acc = eth_account.Account.from_key(private_key)
+        ret = cls(acc.address)
+        ret._private_key = bytes(acc.key)
+        return ret
+
+    @classmethod
+    def from_mnemonic(
+        cls,
+        mnemonic: str,
+        passphrase: str = "",
+        path: str = "m/44'/60'/0'/0/0",
+    ) -> Address:
+        acc = eth_account.Account.from_mnemonic(mnemonic, passphrase, path)
+        ret = cls(acc.address)
+        ret._private_key = bytes(acc.key)
+        return ret
+
+    @classmethod
+    def from_alias(
+        cls,
+        alias: str,
+        password: Optional[str] = None,
+        keystore: Optional[PathLike] = None,
+    ) -> Address:
+        if keystore is None:
+            path = Path(get_config().global_data_path) / "keystore"
+        else:
+            path = Path(keystore)
+        if not path.is_dir():
+            raise ValueError(f"Keystore path {path} is not a directory")
+
+        path = path / f"{alias}.json"
+        if not path.exists():
+            raise ValueError(f"Alias {alias} not found in keystore {path}")
+
+        with path.open() as f:
+            data = json.load(f)
+
+        if not data["address"].startswith("0x"):
+            data["address"] = "0x" + data["address"]
+
+        if password is None:
+            import click
+
+            password = click.prompt(
+                f"Password for account {alias}", default="", hide_input=True
+            )
+
+        key = eth_account.Account.decrypt(data, password)
+
+        ret = cls(data["address"])
+        ret._private_key = bytes(key)
+        return ret
+
+    @property
+    def private_key(self) -> Optional[bytes]:
+        return self._private_key
+
 
 Address.ZERO = Address(0)
 
 
 @functools.total_ordering
 class Account:
     _address: Address
@@ -360,81 +414,45 @@
 
     def __hash__(self) -> int:
         return hash((self._address, self._chain))
 
     @classmethod
     def new(cls, chain: Optional[Chain] = None) -> Account:
         acc = eth_account.Account.create()
-        ret = cls(acc.address, chain)
-        ret.chain._private_keys[ret.address] = bytes(acc.key)
-        return ret
+        return cls(Address.from_key(acc.key), chain)
 
     @classmethod
     def from_key(
         cls, private_key: Union[str, int, bytes], chain: Optional[Chain] = None
     ) -> Account:
-        acc = eth_account.Account.from_key(private_key)
-        ret = cls(acc.address, chain)
-        ret.chain._private_keys[ret.address] = bytes(acc.key)
-        return ret
+        return cls(Address.from_key(private_key), chain)
 
     @classmethod
     def from_mnemonic(
         cls,
         mnemonic: str,
         passphrase: str = "",
         path: str = "m/44'/60'/0'/0/0",
         chain: Optional[Chain] = None,
     ) -> Account:
-        acc = eth_account.Account.from_mnemonic(mnemonic, passphrase, path)
-        ret = cls(acc.address, chain)
-        ret.chain._private_keys[ret.address] = bytes(acc.key)
-        return ret
+        return cls(Address.from_mnemonic(mnemonic, passphrase, path), chain)
 
     @classmethod
     def from_alias(
         cls,
         alias: str,
         password: Optional[str] = None,
         keystore: Optional[PathLike] = None,
         chain: Optional[Chain] = None,
     ) -> Account:
-        if keystore is None:
-            path = Path(get_config().global_data_path) / "keystore"
-        else:
-            path = Path(keystore)
-        if not path.is_dir():
-            raise ValueError(f"Keystore path {path} is not a directory")
-
-        path = path / f"{alias}.json"
-        if not path.exists():
-            raise ValueError(f"Alias {alias} not found in keystore {path}")
-
-        with path.open() as f:
-            data = json.load(f)
-
-        if not data["address"].startswith("0x"):
-            data["address"] = "0x" + data["address"]
-
-        if password is None:
-            import click
-
-            password = click.prompt(
-                f"Password for account {alias}", default="", hide_input=True
-            )
-
-        key = eth_account.Account.decrypt(data, password)
-
-        ret = cls(data["address"], chain)
-        ret.chain._private_keys[ret.address] = bytes(key)
-        return ret
+        return cls(Address.from_alias(alias, password, keystore), chain)
 
     @property
     def private_key(self) -> Optional[bytes]:
-        return self._chain._private_keys.get(self._address, None)
+        return self._address.private_key
 
     @property
     def address(self) -> Address:
         return self._address
 
     @property
     def label(self) -> Optional[str]:
@@ -750,15 +768,15 @@
             access_list,
             type,
         )
         tx_params = self._chain._build_transaction(
             RequestType.CALL, tx_params, [], None
         )
 
-        tx_hash = self._chain._send_transaction(tx_params)
+        tx_hash = self._chain._send_transaction(tx_params, from_)
 
         if "type" not in tx_params:
             from .transactions import LegacyTransaction
 
             tx_type = LegacyTransaction[bytearray]
         elif tx_params["type"] == 1:
             from .transactions import Eip2930Transaction
@@ -779,15 +797,17 @@
             self.chain,
         )
 
         coverage_handler = get_coverage_handler()
         if coverage_handler is not None:
             tx._fetch_debug_trace_transaction()
             coverage_handler.add_coverage(
-                tx_params, self._chain, tx._debug_trace_transaction
+                tx_params,
+                self._chain,
+                tx._debug_trace_transaction,  # pyright: ignore reportGeneralTypeIssues
             )
 
         if confirmations != 0:
             tx.wait(confirmations)
 
             if self._chain.tx_callback is not None:
                 self._chain.tx_callback(tx)
@@ -798,39 +818,39 @@
         return tx
 
     def sign(self, data: bytes) -> bytes:
         """
         Sign raw data according to EIP-191 type 0x45.
         Specifically, sign(keccak256(b"\x19Ethereum Signed Message:\n" + len(data) + data)) is returned.
         """
-        if self._address not in self._chain._private_keys:
+        if self.private_key is None:
             return self._chain.chain_interface.sign(str(self._address), data)
         else:
             return bytes(
                 eth_account.Account.sign_message(
                     eth_account.messages.encode_defunct(data),
-                    self._chain._private_keys[self._address],
+                    self.private_key,
                 ).signature
             )
 
     def sign_hash(self, data_hash: bytes) -> bytes:
         """
         Sign any 32B data (typically keccak256 hash) without prepending any prefix (non EIP-191 compliant).
         This is not recommended for most use cases.
         Specifically, sign(data_hash) is returned.
         """
-        if self._address not in self._chain._private_keys:
+        if self.private_key is None:
             raise NotImplementedError(
                 "Signing data hash without prefix (non EIP-191 compliant) is not supported for accounts without supplied private key"
             )
         else:
             return bytes(
                 eth_account.Account.signHash(
                     data_hash,
-                    self._chain._private_keys[self._address],
+                    self.private_key,
                 ).signature
             )
 
     def _prepare_eip712_dict(
         self, message: Any, domain: Eip712Domain, client_signing: bool
     ) -> Dict[str, Any]:
         def _get_type(t: Type, options: Optional[Dict[str, Any]] = None) -> str:
@@ -978,17 +998,17 @@
         self, message: Any, domain: Optional[Eip712Domain] = None
     ) -> bytes:
         """
         Sign structured data according to EIP-712. Message can be either a raw dictionary as described in the EIP
         (https://eips.ethereum.org/EIPS/eip-712), or any ABI-compatible dataclass.
         """
 
-        client_signing = self._address not in self._chain._private_keys
+        client_signing = self.private_key is None
 
-        if isinstance(message, collections.MutableMapping):
+        if isinstance(message, dict):
             if domain is not None:
                 raise ValueError(
                     "Domain cannot be specified when message is a dictionary"
                 )
         else:
             if domain is None:
                 raise ValueError(
@@ -998,15 +1018,15 @@
 
         if client_signing:
             return self._chain.chain_interface.sign_typed(str(self._address), message)
         else:
             return bytes(
                 eth_account.Account.sign_message(
                     eth_account.messages.encode_structured_data(message),
-                    self._chain._private_keys[self._address],
+                    self.private_key,
                 ).signature
             )
 
 
 Eip712Domain = TypedDict(
     "Eip712Domain",
     {
@@ -1031,29 +1051,28 @@
 
 
 class Chain(ABC):
     _connected: bool
     _chain_interface: ChainInterfaceAbc
     _accounts: List[Account]
     _accounts_set: Set[Account]  # for faster lookup
-    _nonces: KeyedDefaultDict[Address, int]  # pyright: reportGeneralTypeIssues=false
+    _nonces: KeyedDefaultDict[Address, int]  # pyright: ignore reportGeneralTypeIssues
     _default_call_account: Optional[Account]
     _default_tx_account: Optional[Account]
     _default_estimate_account: Optional[Account]
     _default_access_list_account: Optional[Account]
     _default_tx_type: int
     _default_tx_confirmations: int
     _deployed_libraries: DefaultDict[bytes, List[Library]]
     _single_source_errors: Set[bytes]
     _snapshots: Dict[str, Dict]
     _blocks: ChainBlocks
     _txs: ChainTransactions
     _chain_id: int
     _labels: Dict[Address, str]
-    _private_keys: Dict[Address, bytes]
     _require_signed_txs: bool
     _fork: Optional[str]
     _debug_trace_call_supported: bool
     _client_version: str
 
     tx_callback: Optional[Callable[[TransactionAbc], None]]
 
@@ -1121,15 +1140,15 @@
         ...
 
     @max_priority_fee_per_gas.setter
     @abstractmethod
     def max_priority_fee_per_gas(self, value: int) -> None:
         ...
 
-    @contextmanager
+    @contextmanager  # pyright: ignore reportGeneralTypeIssues
     @abstractmethod
     def connect(
         self,
         uri: Optional[str] = None,
         *,
         accounts: Optional[int] = None,
         chain_id: Optional[int] = None,
@@ -1255,30 +1274,29 @@
             self._txs = ChainTransactions(self)
 
             self._accounts = [
                 Account(acc, self) for acc in self._chain_interface.get_accounts()
             ]
             self._accounts_set = set(self._accounts)
             self._nonces = KeyedDefaultDict(
-                lambda addr: self._chain_interface.get_transaction_count(
+                lambda addr: self._chain_interface.get_transaction_count(  # pyright: ignore reportGeneralTypeIssues
                     str(addr)
-                )  # pyright: reportGeneralTypeIssues=false
+                )
             )
             self._snapshots = {}
             self._deployed_libraries = defaultdict(list)
             self._default_call_account = (
                 self._accounts[0] if len(self._accounts) > 0 else None
             )
             self._default_tx_account = None
             self._default_estimate_account = None
             self._default_access_list_account = None
             self._default_tx_confirmations = 1
             self._blocks = ChainBlocks(self)
             self._labels = {}
-            self._private_keys = {}
             self._fork = fork
 
             self._single_source_errors = {
                 selector
                 for selector, sources in errors.items()
                 if len({source for fqn, source in sources.items()}) == 1
             }
@@ -1663,16 +1681,16 @@
             try:
                 fqn_overrides: ChainMap[Address, Optional[str]] = ChainMap()
                 for i in range(tx.tx_index):
                     prev_tx = tx.block.txs[i]
                     prev_tx._fetch_debug_trace_transaction()
                     process_debug_trace_for_fqn_overrides(
                         prev_tx,
-                        prev_tx._debug_trace_transaction,
-                        fqn_overrides,  # pyright: reportGeneralTypeIssues=false
+                        prev_tx._debug_trace_transaction,  # pyright: ignore reportGeneralTypeIssues
+                        fqn_overrides,
                     )
                 fqn = process_debug_trace_for_revert(tx, debug_trace, fqn_overrides)
             except ValueError:
                 raise UnknownTransactionRevertedError(revert_data) from None
         else:
             fqn = list(errors[selector].keys())[0]
 
@@ -1721,16 +1739,16 @@
             )
             fqn_overrides: ChainMap[Address, Optional[str]] = ChainMap()
             for i in range(tx.tx_index):
                 prev_tx = tx.block.txs[i]
                 prev_tx._fetch_debug_trace_transaction()
                 process_debug_trace_for_fqn_overrides(
                     prev_tx,
-                    prev_tx._debug_trace_transaction,
-                    fqn_overrides,  # pyright: reportGeneralTypeIssues=false
+                    prev_tx._debug_trace_transaction,  # pyright: ignore reportGeneralTypeIssues
+                    fqn_overrides,
                 )
             event_traces = process_debug_trace_for_events(
                 tx, debug_trace, fqn_overrides
             )
             assert len(event_traces) == len(logs)
         else:
             event_traces = [(None, None)] * len(logs)
@@ -1895,31 +1913,39 @@
             raise e from None
 
         if revert_data.startswith("0x"):
             revert_data = revert_data[2:]
 
         self._process_revert_data(None, bytes.fromhex(revert_data))
 
-    def _send_transaction(self, tx_params: TxParams) -> str:
+    def _send_transaction(
+        self, tx_params: TxParams, from_: Optional[Union[Account, Address, str]]
+    ) -> str:
         assert "from" in tx_params
         assert "nonce" in tx_params
 
         if self._chain_id in {56, 97}:
-            # BSC doesn't support access lists and tx type
-            del tx_params["type"]
-            del tx_params["accessList"]
+            # BSC doesn't support access lists and tx type            
+            tx_params.pop("type", None)
+            tx_params.pop("accessList", None)            
 
         self._confirm_transaction(tx_params)
 
         if self.require_signed_txs:
-            key = self._private_keys.get(Address(tx_params["from"]), None)
-            tx_params["from"] = eth_utils.to_checksum_address(tx_params["from"])
+            if isinstance(from_, (Account, Address)):
+                key = from_.private_key
+            elif from_ is None and self._default_tx_account is not None:
+                key = self._default_tx_account.private_key
+            else:
+                key = None
+
+            tx_params["from"] = eth_utils.address.to_checksum_address(tx_params["from"])
 
             if "to" in tx_params:
-                tx_params["to"] = eth_utils.to_checksum_address(tx_params["to"])
+                tx_params["to"] = eth_utils.address.to_checksum_address(tx_params["to"])
 
             if Account(tx_params["from"], self) in self._accounts_set:
                 try:
                     tx_hash = self._chain_interface.send_transaction(tx_params)
                 except (ValueError, JsonRpcError) as e:
                     try:
                         tx_hash = e.args[0]["data"]["txHash"]
@@ -2040,18 +2066,19 @@
         self,
         abi: Optional[Dict],
         arguments: Iterable,
         params: TxParams,
         return_tx: bool,
         return_type: Type,
         confirmations: Optional[int],
+        from_: Optional[Union[Account, Address, str]],
     ) -> Any:
         tx_params = self._build_transaction(RequestType.TX, params, arguments, abi)
 
-        tx_hash = self._send_transaction(tx_params)
+        tx_hash = self._send_transaction(tx_params, from_)
 
         if "type" not in tx_params:
             from woke.development.transactions import LegacyTransaction
 
             tx_type = LegacyTransaction[return_type]
         elif tx_params["type"] == 1:
             from woke.development.transactions import Eip2930Transaction
@@ -2071,15 +2098,19 @@
             return_type,
             self,
         )
 
         coverage_handler = get_coverage_handler()
         if coverage_handler is not None:
             tx._fetch_debug_trace_transaction()
-            coverage_handler.add_coverage(tx_params, self, tx._debug_trace_transaction)
+            coverage_handler.add_coverage(
+                tx_params,
+                self,
+                tx._debug_trace_transaction,  # pyright: ignore reportGeneralTypeIssues
+            )
 
         if confirmations != 0:
             tx.wait(confirmations)
 
             if self.tx_callback is not None:
                 self.tx_callback(tx)
 
@@ -2647,14 +2678,15 @@
             return chain._transact(
                 abi,
                 arguments,
                 params,
                 return_tx,
                 return_type,
                 confirmations,
+                from_,
             )
         elif request_type == RequestType.CALL:
             if block is None:
                 block = "latest"
             return chain._call(abi, arguments, params, return_type, block)
         elif request_type == RequestType.ESTIMATE:
             if block is None:
```

### Comparing `woke-3.3.0/woke/development/globals.py` & `woke-3.4.0/woke/development/globals.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/hardhat_console.py` & `woke-3.4.0/woke/development/hardhat_console.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/internal.py` & `woke-3.4.0/woke/development/internal.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/json_rpc/communicator.py` & `woke-3.4.0/woke/development/json_rpc/communicator.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/json_rpc/http.py` & `woke-3.4.0/woke/development/json_rpc/http.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/json_rpc/ipc.py` & `woke-3.4.0/woke/development/json_rpc/ipc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import platform
 import time
 
 from .abc import ProtocolAbc
 
 if platform.system() == "Windows":
-    import win32file  # pyright: reportMissingImports=false
+    import win32file  # pyright: ignore reportMissingModuleSource
 
-    class IpcProtocol(ProtocolAbc):  # pyright: reportGeneralTypeIssues=false
+    class IpcProtocol(ProtocolAbc):  # pyright: ignore reportGeneralTypeIssues
         _uri: str
         _timeout: float
 
         def __init__(self, uri: str, timeout: float):
             self._uri = uri
             self._timeout = timeout
 
@@ -26,21 +26,26 @@
                 None,
             )
 
         def __exit__(self, exc_type, exc_val, exc_tb):
             self._handle.close()
 
         def send_recv(self, data: str):
-            win32file.WriteFile(self._handle, data.encode("utf-8"))
+            win32file.WriteFile(
+                self._handle,  # pyright: ignore reportGeneralTypeIssues
+                data.encode("utf-8"),
+            )
             received = bytearray()
             start = time.perf_counter()
 
             while time.perf_counter() - start < self._timeout:
-                res, data = win32file.ReadFile(self._handle, 4096)
-                received += data  # pyright: reportGeneralTypeIssues=false
+                res, data = win32file.ReadFile(
+                    self._handle, 4096  # pyright: ignore reportGeneralTypeIssues
+                )
+                received += data  # pyright: ignore reportGeneralTypeIssues
                 if not received.rstrip().endswith((b"}", b"]")):
                     continue
                 try:
                     return json.loads(received.decode("utf-8"))
                 except json.JSONDecodeError:
                     continue
             raise TimeoutError("IPC communication timeout")
```

### Comparing `woke-3.3.0/woke/development/json_rpc/websocket.py` & `woke-3.4.0/woke/development/json_rpc/websocket.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/primitive_types.py` & `woke-3.4.0/woke/development/primitive_types.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/development/pytypes_generator.py` & `woke-3.4.0/woke/development/pytypes_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     ignore = False
 
     for i, opcode in enumerate(opcodes_spl):
         if ignore:
             ignore = False
             continue
 
-        if not opcode.startswith("PUSH"):
+        if not opcode.startswith("PUSH") or opcode == "PUSH0":
             pc_op_map.append((pc, opcode, 1, None))
             pc += 1
         else:
             size = int(opcode[4:]) + 1
             pc_op_map.append((pc, opcode, size, int(opcodes_spl[i + 1], 16)))
             pc += size
             ignore = True
@@ -166,15 +166,16 @@
     __errors_index: Dict[bytes, Dict[str, Any]]
     __events_index: Dict[bytes, Dict[str, Any]]
     __contracts_by_metadata_index: Dict[bytes, str]
     __contracts_inheritance_index: Dict[str, Tuple[str, ...]]
     __contracts_revert_index: Dict[str, Set[int]]
     __creation_code_index: List[Tuple[Tuple[Tuple[int, bytes], ...], str]]
     __line_indexes: Dict[Path, List[Tuple[bytes, int]]]
-    __tx_return_types: DefaultDict[str, Dict[str, str]]
+    # source unit name -> other source unit names in the cycle
+    __cyclic_source_units: DefaultDict[str, Set[str]]
 
     def __init__(self, config: WokeConfig, return_tx_obj: bool):
         self.__config = config
         self.__return_tx_obj = return_tx_obj
         self.__source_unit_types = ""
         self.__already_generated_contracts = set()
         self.__source_units = {}
@@ -191,32 +192,30 @@
         self.__errors_index = {}
         self.__events_index = {}
         self.__contracts_by_metadata_index = {}
         self.__contracts_inheritance_index = {}
         self.__contracts_revert_index = {}
         self.__creation_code_index = []
         self.__line_indexes = {}
-        self.__tx_return_types = defaultdict(dict)
+        self.__cyclic_source_units = defaultdict(set)
 
         # built-in Error(str) and Panic(uint256) errors
         error_abi = {
             "name": "Error",
             "type": "error",
             "inputs": [{"internalType": "string", "name": "message", "type": "string"}],
         }
         panic_abi = {
             "name": "Panic",
             "type": "error",
             "inputs": [{"internalType": "uint256", "name": "code", "type": "uint256"}],
         }
 
         for item in [error_abi, panic_abi]:
-            selector = eth_utils.function_abi_to_4byte_selector(
-                item
-            )  # pyright: reportPrivateImportUsage=false
+            selector = eth_utils.abi.function_abi_to_4byte_selector(item)
             self.__errors_index[selector] = {}
             self.__errors_index[selector][""] = (
                 "woke.development.transactions",
                 (item["name"],),
             )
 
     def __setup_line_indexes(self, file: Path) -> None:
@@ -260,17 +259,21 @@
         self.__sol_to_py_lookup[types.Bytes.__name__] = (
             "Union[bytearray, bytes]",
             "bytearray",
         )
         self.__sol_to_py_lookup[types.Function.__name__] = ("Callable", "Callable")
 
     @property
-    def current_source_unit(self):
+    def current_source_unit(self) -> str:
         return self.__current_source_unit
 
+    @property
+    def cyclic_source_units(self) -> Set[str]:
+        return self.__cyclic_source_units[self.__current_source_unit]
+
     def add_str_to_types(
         self, num_of_indentation: int, string: str, num_of_newlines: int
     ):
         self.__source_unit_types += (
             num_of_indentation * TAB_WIDTH * " " + string + num_of_newlines * "\n"
         )
 
@@ -542,24 +545,20 @@
                         if arg["internalType"].startswith("contract "):
                             arg["type"] = arg["internalType"][9:]
                         elif arg["internalType"].startswith("struct "):
                             arg["type"] = arg["internalType"][7:]
                         elif arg["internalType"].startswith("enum "):
                             arg["type"] = arg["internalType"][5:]
 
-                    selector = eth_utils.function_abi_to_4byte_selector(
-                        item_copy
-                    )  # pyright: reportPrivateImportUsage=false
+                    selector = eth_utils.abi.function_abi_to_4byte_selector(item_copy)
                 else:
-                    selector = eth_utils.function_abi_to_4byte_selector(item)
+                    selector = eth_utils.abi.function_abi_to_4byte_selector(item)
                 abi_by_selector[selector] = item
             elif item["type"] == "error":
-                selector = eth_utils.function_abi_to_4byte_selector(
-                    item
-                )  # pyright: reportPrivateImportUsage=false
+                selector = eth_utils.abi.function_abi_to_4byte_selector(item)
 
                 if selector not in self.__errors_index:
                     self.__errors_index[selector] = {}
 
                 # find where the error is declared
                 error_decl = None
                 for error in contract.used_errors:
@@ -584,17 +583,15 @@
                     self.__errors_index[selector][fqn] = (
                         error_module_name,
                         (self.get_name(error_decl),),
                     )
                 else:
                     raise Exception("Unknown error parent")
             elif item["type"] == "event":
-                selector = eth_utils.event_abi_to_log_topic(
-                    item
-                )  # pyright: reportPrivateImportUsage=false
+                selector = eth_utils.abi.event_abi_to_log_topic(item)
                 events_abi[selector] = item
 
                 event_decl = None
                 for c in contract.linearized_base_contracts:
                     for event in c.events:
                         if event.event_selector == selector:
                             event_decl = event
@@ -762,17 +759,15 @@
             assert used_in.compilation_info is not None
             assert used_in.compilation_info.abi is not None
 
             error_abi = None
 
             for item in used_in.compilation_info.abi:
                 if item["type"] == "error" and item["name"] == error.name:
-                    selector = eth_utils.function_abi_to_4byte_selector(
-                        item
-                    )  # pyright: reportPrivateImportUsage=false
+                    selector = eth_utils.abi.function_abi_to_4byte_selector(item)
                     if selector == error.error_selector:
                         error_abi = item
                         break
 
             assert error_abi is not None
 
             parameters: List[Tuple[str, str, str, str]] = []
@@ -979,14 +974,15 @@
             param_names.append((param_name, param.type_string))
             params.append(
                 f"{param_name}: {self.parse_type_and_import(param.type, False)}"
             )
         return param_names, params
 
     def generate_func_returns(self, fn: FunctionDefinition) -> List[Tuple[str, str]]:
+        self.__imports.clear_tmp_type_checking_imports()
         return [
             (self.parse_type_and_import(par.type, True), par.type_string)
             for par in fn.return_parameters.parameters
         ]
 
     def is_compound_type(self, var_type: types.TypeAbc):
         name = var_type.__class__.__name__
@@ -1165,14 +1161,15 @@
                         self.__sol_to_py_lookup[var_type.__class__.__name__][1],
                         var_type_name.type_string,
                     )
                 ]
 
             return parsed if use_parse else []
 
+        self.__imports.clear_tmp_type_checking_imports()
         generated_params = generate_getter_helper(decl.type_name, False, 0)
 
         if len(returns) == 0:
             returns_str = "None"
         elif len(returns) == 1:
             returns_str = returns[0][0]
         else:
@@ -1275,18 +1272,18 @@
         if len(returns) == 0:
             return_types = "NoneType"
         elif len(returns) == 1:
             return_types = returns[0][0]
         else:
             return_types = f"Tuple[{', '.join(map(itemgetter(0), returns))}]"
 
-        assert isinstance(declaration.parent, ContractDefinition)
-        self.__tx_return_types[self.get_name(declaration.parent)][
-            self.get_name(declaration)
-        ] = return_types
+        for cyclic_import in self.__imports.tmp_type_checking_imports:
+            self.add_str_to_types(2, cyclic_import, 1)
+        if self.__imports.tmp_type_checking_imports:
+            self.add_str_to_types(2, "", 1)
 
         assert declaration.function_selector is not None
         fn_selector = declaration.function_selector.hex()
         self.add_str_to_types(
             2,
             f'return self._execute(self.chain, request_type, "{fn_selector}", [{", ".join(map(itemgetter(0), param_names))}], True if request_type == "tx" else False, {return_types}, from_, to if to is not None else str(self.address), value, gas_limit, gas_price, max_fee_per_gas, max_priority_fee_per_gas, access_list, type, block, confirmations)',
             2,
@@ -1410,15 +1407,15 @@
             if (
                 parent_contract.parent.source_unit_name
                 == contract.parent.source_unit_name
             ):
                 self.generate_types_contract(parent_contract)
             # contract is not in the same source unit, so it must be imported
             else:
-                self.__imports.generate_contract_import(parent_contract)
+                self.__imports.generate_contract_import(parent_contract, force=True)
 
         contract_module_name = "pytypes." + _make_path_alphanum(
             contract.parent.source_unit_name[:-3]
         ).replace("/", ".")
         self.__contracts_index[fqn] = (
             contract_module_name,
             (self.get_name(contract),),
@@ -1462,21 +1459,14 @@
                     )
 
         for fn_name, selector in selector_assignments:
             self.add_str_to_types(
                 0, f"{self.get_name(contract)}.{fn_name}.selector = {selector}", 1
             )
 
-        for contract_name in self.__tx_return_types.keys():
-            for fn_name, return_type in self.__tx_return_types[contract_name].items():
-                self.add_str_to_types(
-                    0, f"{contract_name}.{fn_name}.return_type = {return_type}", 1
-                )
-        self.__tx_return_types.clear()
-
     def generate_types_source_unit(self, unit: SourceUnit) -> None:
         self.generate_types_struct(unit.structs, 0)
         self.generate_types_enum(unit.enums, 0)
         self.generate_types_error(unit.errors, 0)
         for contract in unit.contracts:
             self.generate_types_contract(contract)
 
@@ -1602,56 +1592,81 @@
         self.__reference_resolver = build.reference_resolver
 
         self.clean_type_dir()
 
         # generate source units in import order, source units with no imports are generated first
         # also handle cyclic imports
         assert compiler.latest_graph is not None
-        graph = compiler.latest_graph.copy()
+        graph: nx.DiGraph = (
+            compiler.latest_graph.copy()
+        )  # pyright: ignore reportGeneralTypeIssues
         paths_to_source_unit_names: DefaultDict[Path, Set[str]] = defaultdict(set)
         for source_unit_name, info in build_info.source_units_info.items():
             paths_to_source_unit_names[info.fs_path].add(source_unit_name)
 
         previous_len = len(graph)
         cycles_detected = False
         cycles: Set[FrozenSet[str]] = set()
 
+        for cycle in nx.simple_cycles(graph):
+            for source_unit_name in cycle:
+                self.__cyclic_source_units[source_unit_name].update(
+                    [s for s in cycle if s != source_unit_name]
+                )
+
         while len(graph) > 0:
             # use heapq to make order of source units deterministic
             sources: List[str] = [
-                node for node, in_degree in graph.in_degree() if in_degree == 0
+                node
+                for node, in_degree in graph.in_degree()  # pyright: ignore reportGeneralTypeIssues
+                if in_degree == 0
             ]
             heapq.heapify(sources)
             visited: Set[str] = set(sources)
 
             while len(sources) > 0:
                 source = heapq.heappop(sources)
                 path = build_info.source_units_info[source].fs_path
                 if path in self.__source_units:
                     generate_source_unit(self.__source_units[path])
 
                 for source_unit_name in paths_to_source_unit_names[path]:
                     visited.add(source_unit_name)
-                    for _, to in graph.out_edges(source_unit_name):
-                        if graph.in_degree(to) == 1:
+                    for (
+                        _,
+                        to,
+                    ) in graph.out_edges(  # pyright: ignore reportGeneralTypeIssues
+                        source_unit_name  # pyright: ignore reportGeneralTypeIssues
+                    ):
+                        if (
+                            graph.in_degree(
+                                to  # pyright: ignore reportGeneralTypeIssues
+                            )
+                            == 1
+                        ):
                             heapq.heappush(sources, to)
                             visited.add(to)
                 graph.remove_nodes_from(paths_to_source_unit_names[path])
 
             generated_cycles: Set[FrozenSet[str]] = set()
 
             for cycle in nx.simple_cycles(graph):
                 cycles_detected = True
                 cycles.add(frozenset(cycle))
                 if frozenset(cycle) in generated_cycles:
                     continue
 
                 is_closed_cycle = True
                 for node in cycle:
-                    if any(edge[0] not in cycle for edge in graph.in_edges(node)):
+                    if any(
+                        edge[0] not in cycle
+                        for edge in graph.in_edges(
+                            node  # pyright: ignore reportGeneralTypeIssues
+                        )
+                    ):
                         is_closed_cycle = False
                         break
 
                 if is_closed_cycle:
                     generated_cycles.add(frozenset(cycle))
 
             for cycle in sorted(generated_cycles):
@@ -1688,75 +1703,93 @@
 
 class SourceUnitImports:
     __all_imports: str
     __struct_imports: Set[str]
     __enum_imports: Set[str]
     __contract_imports: Set[str]
     __python_imports: Set[str]
+    __type_checking_imports: Set[str]
+    __tmp_type_checking_imports: Set[str]
     __type_gen: TypeGenerator
 
     def __init__(self, outer: TypeGenerator):
         self.__struct_imports = set()
         self.__enum_imports = set()
         self.__all_imports = ""
         self.__contract_imports = set()
         self.__python_imports = set()
+        self.__type_checking_imports = set()
+        self.__tmp_type_checking_imports = set()
         self.__type_gen = outer
 
     def __str__(self) -> str:
-        self.add_str_to_imports(0, DEFAULT_IMPORTS, 1)
+        self.__add_str_to_imports(0, DEFAULT_IMPORTS, 1)
 
         for python_import in sorted(self.__python_imports):
-            self.add_str_to_imports(0, python_import, 1)
+            self.__add_str_to_imports(0, python_import, 1)
 
         if self.__python_imports:
-            self.add_str_to_imports(0, "", 1)
+            self.__add_str_to_imports(0, "", 1)
 
         for contract in sorted(self.__contract_imports):
-            self.add_str_to_imports(0, contract, 1)
+            self.__add_str_to_imports(0, contract, 1)
 
         if self.__contract_imports:
-            self.add_str_to_imports(0, "", 1)
+            self.__add_str_to_imports(0, "", 1)
 
         for struct in sorted(self.__struct_imports):
-            self.add_str_to_imports(0, struct, 1)
+            self.__add_str_to_imports(0, struct, 1)
 
         if self.__struct_imports:
-            self.add_str_to_imports(0, "", 1)
+            self.__add_str_to_imports(0, "", 1)
 
         for enum in sorted(self.__enum_imports):
-            self.add_str_to_imports(0, enum, 1)
+            self.__add_str_to_imports(0, enum, 1)
 
         if self.__enum_imports:
-            self.add_str_to_imports(0, "", 1)
+            self.__add_str_to_imports(0, "", 1)
 
-        self.add_str_to_imports(0, "", 2)
+        if self.__type_checking_imports:
+            self.__add_str_to_imports(0, "from typing import TYPE_CHECKING", 1)
+            self.__add_str_to_imports(0, "if TYPE_CHECKING:", 1)
+            for type_checking_import in sorted(self.__type_checking_imports):
+                self.__add_str_to_imports(1, type_checking_import, 1)
+            self.__add_str_to_imports(0, "", 1)
+
+        self.__add_str_to_imports(0, "", 2)
 
         return self.__all_imports
 
     def cleanup_imports(self) -> None:
-        self.__struct_imports = set()
-        self.__enum_imports = set()
-        self.__contract_imports = set()
-        self.__python_imports = set()
+        self.__struct_imports.clear()
+        self.__enum_imports.clear()
+        self.__contract_imports.clear()
+        self.__python_imports.clear()
+        self.__type_checking_imports.clear()
         self.__all_imports = ""
 
-    # TODO rename to better represent the functionality
-    def generate_import(
+    def clear_tmp_type_checking_imports(self) -> None:
+        self.__tmp_type_checking_imports.clear()
+
+    @property
+    def tmp_type_checking_imports(self) -> FrozenSet[str]:
+        return frozenset(self.__tmp_type_checking_imports)
+
+    def __generate_import(
         self, declaration: DeclarationAbc, source_unit_name: str
     ) -> str:
         source_unit_name = _make_path_alphanum(source_unit_name)
         return (
             "from pytypes."
             + source_unit_name[:-3].replace("/", ".")
             + " import "
             + self.__type_gen.get_name(declaration)
         )
 
-    def add_str_to_imports(
+    def __add_str_to_imports(
         self, num_of_indentation: int, string: str, num_of_newlines: int
     ):
         self.__all_imports += (
             num_of_indentation * TAB_WIDTH * " " + string + num_of_newlines * "\n"
         )
 
     def generate_struct_import(self, struct_type: types.Struct):
@@ -1764,46 +1797,59 @@
         if isinstance(node.parent, ContractDefinition):
             source_unit = node.parent.parent
         else:
             source_unit = node.parent
         # only those structs that are defined in a different source unit should be imported
         if source_unit.source_unit_name == self.__type_gen.current_source_unit:
             return
-        struct_import = self.generate_import(
+        struct_import = self.__generate_import(
             struct_type.ir_node, source_unit.source_unit_name
         )
 
-        if struct_import not in self.__struct_imports:
-            # self.add_str_to_imports(0, struct_import, 1)
+        if source_unit.source_unit_name in self.__type_gen.cyclic_source_units:
+            self.__type_checking_imports.add(struct_import)
+            self.__tmp_type_checking_imports.add(struct_import)
+        else:
             self.__struct_imports.add(struct_import)
 
     # only used for top-level enums (not within contracts)
     def generate_enum_import(self, enum_type: types.Enum):
         source_unit = enum_type.ir_node.parent
         assert isinstance(source_unit, SourceUnit)
 
         # only those structs that are defined in a different source unit should be imported
         if source_unit.source_unit_name == self.__type_gen.current_source_unit:
             return
-        enum_import = self.generate_import(
+        enum_import = self.__generate_import(
             enum_type.ir_node, source_unit.source_unit_name
         )
 
-        if enum_import not in self.__enum_imports:
-            # self.add_str_to_imports(0, struct_import, 1)
+        if source_unit.source_unit_name in self.__type_gen.cyclic_source_units:
+            self.__type_checking_imports.add(enum_import)
+            self.__tmp_type_checking_imports.add(enum_import)
+        else:
             self.__enum_imports.add(enum_import)
 
-    def generate_contract_import(self, contract: ContractDefinition):
+    def generate_contract_import(
+        self, contract: ContractDefinition, *, force: bool = False
+    ):
         source_unit = contract.parent
         if source_unit.source_unit_name == self.__type_gen.current_source_unit:
             return
 
-        contract_import = self.generate_import(contract, source_unit.source_unit_name)
+        contract_import = self.__generate_import(contract, source_unit.source_unit_name)
 
-        if contract_import not in self.__contract_imports:
+        if (
+            not force
+            and contract_import not in self.__contract_imports
+            and source_unit.source_unit_name in self.__type_gen.cyclic_source_units
+        ):
+            self.__type_checking_imports.add(contract_import)
+            self.__tmp_type_checking_imports.add(contract_import)
+        else:
             self.__contract_imports.add(contract_import)
 
     def add_python_import(self, p_import: str) -> None:
         self.__python_imports.add(p_import)
 
 
 class NameSanitizer:
```

### Comparing `woke-3.3.0/woke/development/transactions.py` & `woke-3.4.0/woke/development/transactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from __future__ import annotations
 
 import functools
 import importlib
 import inspect
 from abc import ABC, abstractmethod
-from contextlib import AbstractContextManager, contextmanager
+from contextlib import contextmanager
 from dataclasses import dataclass, field, fields
 from enum import IntEnum
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     Dict,
     Generic,
+    Iterator,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 from urllib.error import HTTPError
 
+from typing_extensions import get_args, get_origin, get_type_hints
+
 if TYPE_CHECKING:
     from .blocks import Block
 
 from .call_trace import CallTrace
 from .chain_interfaces import (
     AnvilChainInterface,
     GanacheChainInterface,
@@ -112,27 +116,34 @@
                 fqn = get_fqn_from_address(
                     Address(tx_params["to"]),
                     int(tx_data["blockNumber"], 16) - 1
                     if "blockNumber" in tx_data
                     else "latest",
                     self._chain,
                 )
-                module_name, attrs = get_contract_from_fqn(fqn)
+                module_name, attrs = get_contract_from_fqn(
+                    fqn  # pyright: ignore reportGeneralTypeIssues
+                )
                 obj = getattr(importlib.import_module(module_name), attrs[0])
                 for attr in attrs[1:]:
                     obj = getattr(obj, attr)
                 selector = tx_params["data"][:4]
                 abi = obj._abi[selector]
                 method = next(
                     getattr(obj, m)
                     for m in dir(obj)
                     if hasattr(getattr(obj, m), "selector")
                     and getattr(obj, m).selector == selector
                 )
-                return_type = method.return_type
+                return_types = get_args(get_type_hints(method)["return"])
+                return_type = next(
+                    get_args(t)[0]
+                    for t in return_types
+                    if get_origin(t) is TransactionAbc
+                )
             except (KeyError, StopIteration):
                 abi = None
                 return_type = bytearray
         else:
             try:
                 fqn = get_fqn_from_creation_code(tx_params["data"])[0]
                 module_name, attrs = get_contract_from_fqn(fqn)
@@ -217,85 +228,102 @@
     @_fetch_tx_receipt
     def block(self) -> Block:
         return self._chain.blocks[self.block_number]
 
     @property
     @_fetch_tx_receipt
     def block_number(self) -> int:
-        return int(self._tx_receipt["blockNumber"], 16)
+        return int(
+            self._tx_receipt["blockNumber"],  # pyright: ignore reportOptionalSubscript
+            16,
+        )
 
     @property
     def data(self) -> bytes:
         return self._tx_params["data"] if "data" in self._tx_params else b""
 
     @property
     def from_(self) -> Account:
         return Account(
-            self._tx_params["from"], self._chain
-        )  # pyright: reportTypedDictNotRequiredAccess=false
+            self._tx_params["from"],  # pyright: ignore reportTypedDictNotRequiredAccess
+            self._chain,
+        )
 
     @property
     def to(self) -> Optional[Account]:
         if "to" in self._tx_params:
             return Account(self._tx_params["to"], self._chain)
         return None
 
     @property
     def gas_limit(self) -> int:
-        return self._tx_params["gas"]  # pyright: reportTypedDictNotRequiredAccess=false
+        return self._tx_params[
+            "gas"
+        ]  # pyright: ignore reportTypedDictNotRequiredAccess
 
     @property
     def nonce(self) -> int:
         return self._tx_params[
             "nonce"
-        ]  # pyright: reportTypedDictNotRequiredAccess=false
+        ]  # pyright: ignore reportTypedDictNotRequiredAccess
 
     @property
     @_fetch_tx_receipt
     def tx_index(self) -> int:
         return int(
-            self._tx_receipt["transactionIndex"], 16
-        )  # pyright: reportOptionalSubscript=false
+            self._tx_receipt[  # pyright: ignore reportOptionalSubscript
+                "transactionIndex"
+            ],
+            16,
+        )
 
     @property
     def value(self) -> Wei:
         return Wei(
-            self._tx_params["value"]
-        )  # pyright: reportTypedDictNotRequiredAccess=false
+            self._tx_params["value"]  # pyright: ignore reportTypedDictNotRequiredAccess
+        )
 
     @property
     @_fetch_tx_data
     def r(self) -> int:
-        return int(self._tx_data["r"], 16)  # pyright: reportOptionalSubscript=false
+        return int(self._tx_data["r"], 16)  # pyright: ignore reportOptionalSubscript
 
     @property
     @_fetch_tx_data
     def s(self) -> int:
-        return int(self._tx_data["s"], 16)  # pyright: reportOptionalSubscript=false
+        return int(self._tx_data["s"], 16)  # pyright: ignore reportOptionalSubscript
 
     @property
     @_fetch_tx_receipt
     def gas_used(self) -> int:
         return int(
-            self._tx_receipt["gasUsed"], 16
-        )  # pyright: reportOptionalSubscript=false
+            self._tx_receipt["gasUsed"], 16  # pyright: ignore reportOptionalSubscript
+        )
 
     @property
     @_fetch_tx_receipt
     def cumulative_gas_used(self) -> int:
         return int(
-            self._tx_receipt["cumulativeGasUsed"], 16
-        )  # pyright: reportOptionalSubscript=false
+            self._tx_receipt[  # pyright: ignore reportOptionalSubscript
+                "cumulativeGasUsed"
+            ],
+            16,
+        )
 
     @property
     @_fetch_tx_receipt
     def effective_gas_price(self) -> Wei:
         return Wei(
-            int(self._tx_receipt["effectiveGasPrice"], 16)
-        )  # pyright: reportOptionalSubscript=false
+            int(
+                self._tx_receipt[  # pyright: ignore reportOptionalSubscript
+                    "effectiveGasPrice"
+                ],
+                16,
+            )
+        )
 
     @property
     def status(self) -> TransactionStatusEnum:
         if self._tx_receipt is None:
             receipt = self._chain.chain_interface.get_transaction_receipt(self._tx_hash)
             if receipt is None:
                 return TransactionStatusEnum.PENDING
@@ -335,28 +363,28 @@
             return self._chain._process_console_logs(self._trace_transaction)
         elif isinstance(
             chain_interface, (GanacheChainInterface, HardhatChainInterface)
         ):
             self._fetch_debug_trace_transaction()
             assert self._debug_trace_transaction is not None
             return self._chain._process_console_logs_from_debug_trace(
-                self._debug_trace_transaction
+                self._debug_trace_transaction  # pyright: ignore reportGeneralTypeIssues
             )
         elif isinstance(chain_interface, GethLikeChainInterfaceAbc):
             try:
                 self._fetch_trace_transaction()
                 assert self._trace_transaction is not None
                 return self._chain._process_console_logs(self._trace_transaction)
             except (JsonRpcError, HTTPError):
                 # TODO make assertions about error.code?
                 try:
                     self._fetch_debug_trace_transaction()
                     assert self._debug_trace_transaction is not None
                     return self._chain._process_console_logs_from_debug_trace(
-                        self._debug_trace_transaction
+                        self._debug_trace_transaction  # pyright: ignore reportGeneralTypeIssues
                     )
                 except (JsonRpcError, HTTPError):
                     # TODO make assertions about error.code?
                     raise RuntimeError(
                         f"Could not get console logs for transaction {self.tx_hash} as trace_transaction and debug_trace_transaction are both unavailable"
                     )
         else:
@@ -423,14 +451,15 @@
         if self._raw_error is not None:
             return self._raw_error
 
         chain_interface = self._chain.chain_interface
 
         if isinstance(chain_interface, AnvilChainInterface):
             self._fetch_trace_transaction()
+            assert self._trace_transaction is not None
             revert_data = bytes.fromhex(
                 self._trace_transaction[0]["result"]["output"][2:]
             )
         elif isinstance(chain_interface, GanacheChainInterface):
             self._fetch_debug_trace_transaction()
             assert self._debug_trace_transaction is not None
 
@@ -473,15 +502,15 @@
 
     @property
     @_fetch_tx_receipt
     def return_value(self) -> T:
         raw_value = self.raw_return_value
 
         if self._return_type is type(None):
-            return None
+            return None  # pyright: ignore reportGeneralTypeIssues
 
         if isinstance(raw_value, Account):
             return self._return_type(raw_value.address, self._chain)
         elif isinstance(raw_value, bytearray):
             if self._abi is None:
                 return self._return_type(raw_value)
 
@@ -557,29 +586,29 @@
     def call_trace(self) -> CallTrace:
         if self._debug_trace_transaction is None:
             self._fetch_debug_trace_transaction()
         assert self._debug_trace_transaction is not None
 
         return CallTrace.from_debug_trace(
             self,
-            self._debug_trace_transaction,
+            self._debug_trace_transaction,  # pyright: ignore reportGeneralTypeIssues
             self._tx_params,
-        )  # pyright: reportGeneralTypeIssues=false
+        )
 
     @property
     @abstractmethod
     def type(self) -> TransactionTypeEnum:
         ...
 
 
 class LegacyTransaction(TransactionAbc[T]):
     @property
     @_fetch_tx_data
     def v(self) -> int:
-        return int(self._tx_data["v"], 16)  # pyright: reportOptionalSubscript=false
+        return int(self._tx_data["v"], 16)  # pyright: ignore reportOptionalSubscript
 
     @property
     def gas_price(self) -> Wei:
         assert "gasPrice" in self._tx_params
         return Wei(self._tx_params["gasPrice"])
 
     @property
@@ -608,15 +637,17 @@
     def gas_price(self) -> Wei:
         assert "gasPrice" in self._tx_params
         return Wei(self._tx_params["gasPrice"])
 
     @property
     @_fetch_tx_data
     def y_parity(self) -> bool:
-        return bool(int(self._tx_data["v"], 16) & 1)
+        return bool(
+            int(self._tx_data["v"], 16) & 1  # pyright: ignore reportOptionalSubscript
+        )
 
     @property
     def type(self) -> TransactionTypeEnum:
         assert "type" in self._tx_params and self._tx_params["type"] == 1
         return TransactionTypeEnum.EIP2930
 
 
@@ -656,15 +687,17 @@
                 ret[account] = []
             ret[account].append(entry[1])
         return ret
 
     @property
     @_fetch_tx_data
     def y_parity(self) -> bool:
-        return bool(int(self._tx_data["v"], 16) & 1)
+        return bool(
+            int(self._tx_data["v"], 16) & 1  # pyright: ignore reportOptionalSubscript
+        )
 
     @property
     def type(self) -> TransactionTypeEnum:
         assert "type" in self._tx_params and self._tx_params["type"] == 2
         return TransactionTypeEnum.EIP1559
 
 
@@ -734,61 +767,76 @@
 
 
 @contextmanager
 def must_revert(
     exceptions: Union[
         Exception, Type[Exception], Tuple[Union[Exception, Type[Exception]], ...]
     ] = TransactionRevertedError,
-) -> AbstractContextManager[ExceptionWrapper]:
+) -> Iterator[ExceptionWrapper]:
     if isinstance(exceptions, (tuple, list)):
-        types = tuple(
-            type(x) if not inspect.isclass(x) else x for x in exceptions
-        )  # pyright: reportGeneralTypeIssues=false
+        types = tuple(type(x) if not inspect.isclass(x) else x for x in exceptions)
     else:
         types = type(exceptions) if not inspect.isclass(exceptions) else exceptions
 
     wrapper = ExceptionWrapper()
 
     try:
         yield wrapper
         raise AssertionError(f"Expected revert of type {exceptions}")
-    except types as e:  # pyright: reportGeneralTypeIssues=false
+    except types as e:  # pyright: ignore reportGeneralTypeIssues
         wrapper.value = e
 
         if isinstance(exceptions, (tuple, list)):
             for ex, t in zip(
-                exceptions, types
-            ):  # pyright: reportGeneralTypeIssues=false
+                exceptions, types  # pyright: ignore reportGeneralTypeIssues
+            ):
                 if isinstance(ex, t) and not inspect.isclass(ex):
                     assert e == ex, f"Expected {ex} but got {e}"
                     return
         else:
             if not inspect.isclass(exceptions):
                 assert e == exceptions, f"Expected {e} but got {exceptions}"
 
 
 @contextmanager
 def may_revert(
     exceptions: Union[
         Exception, Type[Exception], Tuple[Union[Exception, Type[Exception]], ...]
     ] = TransactionRevertedError,
-) -> AbstractContextManager[ExceptionWrapper]:
+) -> Iterator[ExceptionWrapper]:
     if isinstance(exceptions, (tuple, list)):
         types = tuple(type(x) if not inspect.isclass(x) else x for x in exceptions)
     else:
         types = type(exceptions) if not inspect.isclass(exceptions) else exceptions
 
     wrapper = ExceptionWrapper()
 
     try:
         yield wrapper
-    except types as e:
+    except types as e:  # pyright: ignore reportGeneralTypeIssues
         wrapper.value = e
 
         if isinstance(exceptions, (tuple, list)):
-            for ex, t in zip(exceptions, types):
+            for ex, t in zip(
+                exceptions, types  # pyright: ignore reportGeneralTypeIssues
+            ):
                 if isinstance(ex, t) and not inspect.isclass(ex):
                     assert e == ex, f"Expected {ex} but got {e}"
                     return
         else:
             if not inspect.isclass(exceptions):
                 assert e == exceptions, f"Expected {e} but got {exceptions}"
+
+
+def on_revert(callback: Callable[[TransactionRevertedError], None]):
+    def decorator(f):
+        @functools.wraps(f)
+        def wrapper(*args, **kwargs):
+            try:
+                return f(*args, **kwargs)
+            except TransactionRevertedError as e:
+                callback(e)
+                raise
+
+        return wrapper
+
+    return decorator
```

### Comparing `woke-3.3.0/woke/development/utils.py` & `woke-3.4.0/woke/development/utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/commands/generate_control_flow_graph.py` & `woke-3.4.0/woke/lsp/commands/generate_control_flow_graph.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,54 +52,65 @@
     g.attr(rankdir=context.config.generator.control_flow_graph.direction)
     g.attr("node", shape="box")
 
     skip_start_block = False
     if (
         len(cfg.start_block.statements) == 0
         and cfg.start_block.control_statement is None
-        and graph.out_degree(cfg.start_block) == 1
+        and graph.out_degree(cfg.start_block)  # pyright: ignore reportGeneralTypeIssues
+        == 1
     ):
         skip_start_block = True
 
     skip_end_block = False
     if (
         len(cfg.end_block.statements) == 0
         and cfg.end_block.control_statement is None
-        and graph.in_degree(cfg.end_block) == 1
+        and graph.in_degree(cfg.end_block)  # pyright: ignore reportGeneralTypeIssues
+        == 1
     ):
         skip_end_block = True
 
-    for node in graph.nodes:
+    for node in graph.nodes:  # pyright: ignore reportGeneralTypeIssues
         if skip_start_block and node == cfg.start_block:
             continue
         if skip_end_block and node == cfg.end_block:
             continue
 
         statements: List[StatementAbc] = node.statements
-        node_attrs = {"label": "".join(f"{line}\l" for line in str(node).splitlines())}
+        node_attrs = {
+            "label": "".join(
+                f"{line}\l"  # pyright: ignore reportInvalidStringEscapeSequence
+                for line in str(node).splitlines()
+            )
+        }
         if (
             context.config.generator.control_flow_graph.vscode_urls
             and len(statements) > 0
         ):
             first_statement = statements[0]
             line, column = context.compiler.get_line_pos_from_byte_offset(
                 first_statement.file, first_statement.byte_location[0]
             )
             line += 1
             column += 1
             node_attrs["URL"] = f"vscode://file/{first_statement.file}:{line}:{column}"
         g.node(str(node.id), **node_attrs)
 
-    for from_, to, data in graph.edges.data():
+    for (
+        from_,
+        to,
+        data,
+    ) in graph.edges.data():  # pyright: ignore reportGeneralTypeIssues
         if skip_start_block and from_ == cfg.start_block:
             continue
         if skip_end_block and to == cfg.end_block:
             continue
 
-        condition = data["condition"]
+        condition = data["condition"]  # pyright: ignore reportOptionalSubscript
         if condition[1] is not None:
             label = f"{condition[1].source} {condition[0]}"
         else:
             label = condition[0]
         g.edge(str(from_.id), str(to.id), label=label)
 
     return g.source
```

### Comparing `woke-3.3.0/woke/lsp/commands/generate_imports_graph.py` & `woke-3.4.0/woke/lsp/commands/generate_imports_graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 
     g = gv.Digraph("Imports graph")
     g.attr(rankdir=config.direction)
     g.attr("node", shape="box")
 
     graph = context.compiler.last_graph
 
-    for node in graph.nodes:
+    for node in graph.nodes:  # pyright: ignore reportGeneralTypeIssues
         node_attrs = {}
         if config.vscode_urls:
-            node_attrs["URL"] = f"vscode://file/{graph.nodes[node]['path']}"
+            node_attrs[
+                "URL"
+            ] = f"vscode://file/{graph.nodes[node]['path']}"  # pyright: ignore reportGeneralTypeIssues
         g.node(node, **node_attrs)
 
-    for from_, to in graph.edges:
+    for from_, to in graph.edges:  # pyright: ignore reportGeneralTypeIssues
         if config.imports_direction == ImportsDirection.ImportedToImporting:
             g.edge(from_, to)
         else:
             g.edge(to, from_)
 
     return g.source
```

### Comparing `woke-3.3.0/woke/lsp/commands/generate_inheritance_graph.py` & `woke-3.4.0/woke/lsp/commands/generate_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/commands/generate_linearized_inheritance_graph.py` & `woke-3.4.0/woke/lsp/commands/generate_linearized_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/common_structures.py` & `woke-3.4.0/woke/lsp/common_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1179,17 +1179,24 @@
 
 
 class ClientCapabilitiesGeneralStaleRequestSupport(LspModel):
     cancel: bool
     retry_on_content_modified: List[str]
 
 
+class PositionEncodingKind(StrEnum):
+    UTF8 = "utf-8"
+    UTF16 = "utf-16"
+    UTF32 = "utf-32"
+
+
 class ClientCapabilitiesGeneral(LspModel):
     stale_request_support: Optional[ClientCapabilitiesGeneralStaleRequestSupport]
     regular_expressions: Optional[RegularExpressionsClientCapabilities]
+    position_encodings: Optional[List[PositionEncodingKind]]
     """
     markdown: Optional[MarkdownClientCapabilities]
     """
 
 
 class ClientCapabilitiesWindow(LspModel):
     work_done_progress: Optional[bool]
```

### Comparing `woke-3.3.0/woke/lsp/context.py` & `woke-3.4.0/woke/lsp/context.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,36 +4,39 @@
 from typing import TYPE_CHECKING, Optional
 
 from ..config import WokeConfig
 from ..core.solidity_version import SemanticVersion
 from ..utils.openzeppelin import get_contracts_package_version
 from .features.diagnostic import diagnostics_loop
 from .lsp_compiler import LspCompiler
+from .lsp_parser import LspParser
 
 if TYPE_CHECKING:
     from .server import LspServer
 
 
 class LspContext:
     __server: LspServer
     __workspace_config: WokeConfig
     __compiler: LspCompiler
     __diagnostics_queue: asyncio.Queue
     __openzeppelin_contracts_version: Optional[SemanticVersion]
+    __parser: LspParser
 
     def __init__(
         self, server: LspServer, config: WokeConfig, perform_files_discovery: bool
     ) -> None:
         self.__server = server
         self.__workspace_config = config
         self.__diagnostics_queue = asyncio.Queue()
         self.__compiler = LspCompiler(
             server, self.__diagnostics_queue, perform_files_discovery
         )
         self.__openzeppelin_contracts_version = get_contracts_package_version(config)
+        self.__parser = LspParser(server)
 
     def run(self) -> None:
         self.__server.create_task(diagnostics_loop(self.__server, self))
         self.__server.create_task(self.__compiler.run(self.__workspace_config))
 
     @property
     def config(self) -> WokeConfig:
@@ -50,7 +53,11 @@
     @property
     def server(self) -> LspServer:
         return self.__server
 
     @property
     def openzeppelin_contracts_version(self) -> Optional[SemanticVersion]:
         return self.__openzeppelin_contracts_version
+
+    @property
+    def parser(self) -> LspParser:
+        return self.__parser
```

### Comparing `woke-3.3.0/woke/lsp/document_sync.py` & `woke-3.4.0/woke/lsp/document_sync.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/features/code_lens.py` & `woke-3.4.0/woke/lsp/features/code_lens.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,22 +181,42 @@
 
     code_lens = []
     source_unit = context.compiler.source_units[path]
 
     _code_lens_cache[path] = []
 
     for declaration in source_unit.declarations_iter():
-        refs_count = _resolve_declaration(declaration, context)
+        refs = list(declaration.get_all_references(include_declarations=True))
+        refs_count = len([ref for ref in refs if not isinstance(ref, DeclarationAbc)])
+        declaration_positions = []
+
+        for ref in refs:
+            if isinstance(ref, DeclarationAbc):
+                line, col = context.compiler.get_line_pos_from_byte_offset(
+                    ref.file, ref.name_location[0]
+                )
+                declaration_positions.append(Position(line=line, character=col))
+
+        line, col = context.compiler.get_line_pos_from_byte_offset(
+            declaration.file, declaration.name_location[0]
+        )
+
+        # should include info to be able to recover command args from cache (positions could have changed)
+        # but references do not work in cache mode (compilation error) anyway
         code_lens.append(
             _generate_code_lens(
                 context,
                 declaration.file,
                 f"{refs_count} references" if refs_count != 1 else "1 reference",
-                "",
-                None,
+                "Tools-for-Solidity.execute.references",
+                [
+                    params.text_document.uri,
+                    Position(line=line, character=col),
+                    declaration_positions,
+                ],
                 declaration.name_location,
                 declaration.name_location,
             )
         )
 
         if (
             isinstance(declaration, (FunctionDefinition, ModifierDefinition))
```

### Comparing `woke-3.3.0/woke/lsp/features/definition.py` & `woke-3.4.0/woke/lsp/features/definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/features/diagnostic.py` & `woke-3.4.0/woke/lsp/features/diagnostic.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/features/document_link.py` & `woke-3.4.0/woke/lsp/features/document_link.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import logging
-from pathlib import Path
+from itertools import chain
 from typing import Any, List, Optional
 
+from woke.compiler.exceptions import CompilationResolveError
+from woke.compiler.source_path_resolver import SourcePathResolver
+from woke.compiler.source_unit_name_resolver import SourceUnitNameResolver
 from woke.lsp.common_structures import (
     DocumentUri,
     PartialResultParams,
+    Position,
     Range,
     TextDocumentIdentifier,
     WorkDoneProgressOptions,
     WorkDoneProgressParams,
 )
 from woke.lsp.context import LspContext
 from woke.lsp.lsp_data_model import LspModel
-from woke.lsp.utils.position import changes_to_byte_offset
 from woke.lsp.utils.uri import path_to_uri, uri_to_path
 
 logger = logging.getLogger(__name__)
 
 
 class DocumentLinkOptions(WorkDoneProgressOptions):
     resolve_provider: Optional[bool]
@@ -55,76 +58,74 @@
     data: Optional[Any]
     """
     A data entry field that is preserved on a document link between a
     DocumentLinkRequest and a DocumentLinkResolveRequest.
     """
 
 
-async def _get_document_links_from_cache(path: Path, context: LspContext):
-    source_unit = context.compiler.last_compilation_source_units[path]
-    forward_changes = context.compiler.get_last_compilation_forward_changes(path)
-    if forward_changes is None:
-        raise Exception("No forward changes found for file")
-
-    document_links = []
-
-    for import_directive in source_unit.imports:
-        location = import_directive.import_string_pos
-
-        if len(forward_changes[location[0] : location[1]]) > 0:
-            # change at range, skip import
-            continue
-
-        new_start = (
-            changes_to_byte_offset(forward_changes[0 : location[0]]) + location[0]
-        )
-        new_end = changes_to_byte_offset(forward_changes[0 : location[1]]) + location[1]
-
-        document_links.append(
-            DocumentLink(
-                range=context.compiler.get_range_from_byte_offsets(
-                    path, (new_start, new_end)
-                ),
-                target=DocumentUri(path_to_uri(import_directive.imported_file)),
-                tooltip=None,
-                data=None,
-            )
-        )
-
-    return document_links
-
-
 async def document_link(
     context: LspContext, params: DocumentLinkParams
 ) -> Optional[List[DocumentLink]]:
     logger.debug(f"Requested document links for file {params.text_document.uri}")
 
     path = uri_to_path(params.text_document.uri).resolve()
-    if (
-        path not in context.compiler.source_units
-        or not context.compiler.output_ready.is_set()
+
+    document_links = []
+    source_unit_name_resolver = SourceUnitNameResolver(context.config)
+    source_path_resolver = SourcePathResolver(context.config)
+
+    this_source_unit_name = None
+    for include_path in chain(
+        context.config.compiler.solc.include_paths, [context.config.project_root_path]
     ):
         try:
-            return await _get_document_links_from_cache(path, context)
-        except Exception:
-            pass
+            rel_path = str(path.relative_to(include_path).as_posix())
+            if this_source_unit_name is None or len(this_source_unit_name) > len(
+                rel_path
+            ):
+                this_source_unit_name = rel_path
+        except ValueError:
+            continue
 
-    await context.compiler.output_ready.wait()
-    if path not in context.compiler.source_units:
+    if this_source_unit_name is None:
         return None
 
-    source_unit = context.compiler.source_units[path]
-    document_links = []
+    try:
+        root = context.parser[path].root_node
+    except KeyError:
+        return None
 
-    for import_directive in source_unit.imports:
-        document_links.append(
-            DocumentLink(
-                range=context.compiler.get_range_from_byte_offsets(
-                    path, import_directive.import_string_pos
-                ),
-                target=DocumentUri(path_to_uri(import_directive.imported_file)),
-                tooltip=None,
-                data=None,
-            )
-        )
+    for child in root.children:
+        if child.type == "import_directive":
+            source_node = child.child_by_field_name("source")
+
+            if source_node is not None:
+                import_str = source_node.text.decode("utf-16-le")[1:-1]  # remove quotes
+                unit_name = source_unit_name_resolver.resolve_import(
+                    this_source_unit_name, import_str
+                )
+
+                try:
+                    include_path = source_path_resolver.resolve(
+                        unit_name, this_source_unit_name, context.parser.files
+                    )
+                    document_links.append(
+                        DocumentLink(
+                            range=Range(
+                                start=Position(
+                                    line=source_node.start_point[0],
+                                    character=source_node.start_point[1] // 2,
+                                ),
+                                end=Position(
+                                    line=source_node.end_point[0],
+                                    character=source_node.end_point[1] // 2,
+                                ),
+                            ),
+                            target=DocumentUri(path_to_uri(include_path)),
+                            tooltip=None,
+                            data=None,
+                        )
+                    )
+                except CompilationResolveError:
+                    continue
 
     return document_links
```

### Comparing `woke-3.3.0/woke/lsp/features/document_symbol.py` & `woke-3.4.0/woke/lsp/features/document_symbol.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/features/implementation.py` & `woke-3.4.0/woke/lsp/features/implementation.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/features/references.py` & `woke-3.4.0/woke/lsp/features/references.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/features/rename.py` & `woke-3.4.0/woke/lsp/features/rename.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/features/type_definition.py` & `woke-3.4.0/woke/lsp/features/type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/features/type_hierarchy.py` & `woke-3.4.0/woke/lsp/features/type_hierarchy.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/lsp_compiler.py` & `woke-3.4.0/woke/lsp/lsp_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import difflib
 import logging
+import multiprocessing
+import multiprocessing.connection
 import re
 import threading
 import time
 from collections import deque
 from copy import deepcopy
 from functools import lru_cache
 from pathlib import Path
@@ -94,16 +96,18 @@
     for path in start:
         processed.update(cu.path_to_source_unit_names(path))
     out.update(start)
 
     queue: Deque[str] = deque(processed)
     while len(queue):
         node = queue.pop()
-        for out_edge in cu.graph.out_edges(node):
-            from_, to = out_edge
+        for out_edge in cu.graph.out_edges(
+            node  # pyright: ignore reportGeneralTypeIssues
+        ):
+            from_, to = out_edge  # pyright: ignore reportGeneralTypeIssues
             if to not in processed:
                 processed.add(to)
                 queue.append(to)
                 out.add(cu.source_unit_name_to_path(to))
 
 
 class VersionedFile(NamedTuple):
@@ -347,14 +351,15 @@
                     self.__discovered_files.add(path)
                     self.__force_compile_files.add(path)
         elif isinstance(change, RenameFilesParams):
             for rename in change.files:
                 old_path = uri_to_path(rename.old_uri)
                 self.__deleted_files.add(old_path)
                 self.__discovered_files.discard(old_path)
+                self.__opened_files.pop(old_path, None)
 
                 new_path = uri_to_path(rename.new_uri)
                 if (
                     new_path not in self.__discovered_files
                     and not self.__file_ignored(new_path)
                     and new_path.is_file()
                     and new_path.suffix == ".sol"
@@ -787,15 +792,18 @@
                         self.__last_successful_compilation_contents[
                             path
                         ] = self.__opened_files[path]
                     else:
                         self.__last_successful_compilation_contents[
                             path
                         ] = VersionedFile(
-                            cu.graph.nodes[source_unit_name]["content"], None
+                            cu.graph.nodes[  # pyright: ignore reportGeneralTypeIssues
+                                source_unit_name
+                            ]["content"],
+                            None,
                         )
 
             self.__ir_reference_resolver.run_post_process_callbacks(
                 CallbackParams(
                     interval_trees=self.__interval_trees,
                     source_units=self.__source_units,
                 )
@@ -809,26 +817,44 @@
                 )
 
         if progress_token is not None:
             await self.__server.progress_end(progress_token)
 
         self.__compilation_errors = deepcopy(errors_per_file)
 
-        # diagnostics (compiler errors and warnings + detections) are sent in this function
-        await self.__run_detectors()
+        # send compiler warnings and errors first without waiting for detectors to finish
+        for path, errors in errors_per_file.items():
+            await self.__diagnostic_queue.put((path, errors))
+
+        # run detectors in a separate process
+        parent_conn, child_conn = multiprocessing.Pipe()
+        p = multiprocessing.Process(
+            target=self.__run_detectors,
+            args=(child_conn,),
+        )
+        p.start()
+        while True:
+            if parent_conn.poll():
+                errors_per_file = parent_conn.recv()
+                # send both compiler and detector warnings and errors
+                for path, errors in errors_per_file.items():
+                    await self.__diagnostic_queue.put((path, errors))
+                break
+            elif not p.is_alive():
+                break
+
+            await asyncio.sleep(0.1)
 
         if len(files_to_recompile) > 0:
             # avoid infinite recursion
             if files_to_recompile != files_to_compile or full_compile:
                 await self.__compile(files_to_recompile, False)
 
-    async def __run_detectors(self):
-        errors_per_file: Dict[Path, Set[Diagnostic]] = deepcopy(
-            self.__compilation_errors
-        )
+    def __run_detectors(self, conn: multiprocessing.connection.Connection) -> None:
+        errors_per_file: Dict[Path, Set[Diagnostic]] = self.__compilation_errors
 
         if self.__config.lsp.detectors.enable:
             for detection in detect(self.__config, self.__source_units):
                 file = detection.result.ir_node.file
                 if len(detection.result.related_info) > 0:
                     related_info = [
                         DiagnosticRelatedInformation(
@@ -862,16 +888,15 @@
                         source="Woke",
                         message=detection.result.message,
                         code=detection.code,
                         related_information=related_info,
                     )
                 )
 
-        for path, errors in errors_per_file.items():
-            await self.__diagnostic_queue.put((path, errors))
+        conn.send(errors_per_file)
 
     async def __compilation_loop(self):
         if self.__perform_files_discovery:
             # perform Solidity files discovery
             for file in self.__config.project_root_path.rglob("**/*.sol"):
                 if not self.__file_ignored(file) and file.is_file():
                     self.__discovered_files.add(file.resolve())
@@ -910,15 +935,32 @@
                 )
 
                 self.__force_compile_files.clear()
                 self.__modified_files.clear()
                 self.__deleted_files.clear()
 
             if self.__force_run_detectors:
-                await self.__run_detectors()
+                parent_conn, child_conn = multiprocessing.Pipe()
+                p = multiprocessing.Process(
+                    target=self.__run_detectors,
+                    args=(child_conn,),
+                )
+                p.start()
+                while True:
+                    if parent_conn.poll():
+                        errors_per_file = parent_conn.recv()
+                        # send both compiler and detector warnings and errors
+                        for path, errors in errors_per_file.items():
+                            await self.__diagnostic_queue.put((path, errors))
+                        break
+                    elif not p.is_alive():
+                        break
+
+                    await asyncio.sleep(0.1)
+
                 self.__force_run_detectors = False
 
             if self.__file_changes_queue.empty():
                 self.output_ready.set()
 
     def __setup_line_index(self, file: Path):
         content = self.get_compiled_file(file).text
```

### Comparing `woke-3.3.0/woke/lsp/methods.py` & `woke-3.4.0/woke/lsp/methods.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/protocol_structures.py` & `woke-3.4.0/woke/lsp/protocol_structures.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/rpc_protocol.py` & `woke-3.4.0/woke/lsp/rpc_protocol.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/lsp/server.py` & `woke-3.4.0/woke/lsp/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     ExecuteCommandParams,
     InitializedParams,
     InitializeError,
     InitializeParams,
     LogMessageParams,
     LogTraceParams,
     MessageType,
+    PositionEncodingKind,
     ProgressParams,
     RenameFilesParams,
     SetTraceParams,
     ShowMessageParams,
     WorkDoneProgressBegin,
     WorkDoneProgressCreateParams,
     WorkDoneProgressEnd,
@@ -60,15 +61,17 @@
     DidOpenTextDocumentParams,
     DidSaveTextDocumentParams,
     TextDocumentSyncKind,
     TextDocumentSyncOptions,
     WillSaveTextDocumentParams,
 )
 from .exceptions import LspError
+from .features.code_action import CodeActionOptions, CodeActionParams, code_action
 from .features.code_lens import CodeLensOptions, CodeLensParams, code_lens
+from .features.completion import CompletionOptions, CompletionParams, completion
 from .features.definition import DefinitionParams, definition
 from .features.document_link import (
     DocumentLinkOptions,
     DocumentLinkParams,
     document_link,
 )
 from .features.document_symbol import DocumentSymbolParams, document_symbol
@@ -104,15 +107,14 @@
 from .rpc_protocol import RpcProtocol
 from .server_capabilities import (
     FileOperationFilter,
     FileOperationPattern,
     FileOperationPatternKind,
     FileOperationRegistrationOptions,
     InitializeResult,
-    PositionEncodingKind,
     ServerCapabilities,
     ServerCapabilitiesWorkspace,
     ServerCapabilitiesWorkspaceFileOperations,
     WorkspaceFoldersServerCapabilities,
 )
 from .utils.uri import uri_to_path
 
@@ -209,14 +211,16 @@
             ),
             RequestMethodEnum.RENAME: (self._workspace_route, RenameParams),
             RequestMethodEnum.WORKSPACE_EXECUTE_COMMAND: (
                 self._workspace_execute_command,
                 ExecuteCommandParams,
             ),
             RequestMethodEnum.HOVER: (self._workspace_route, HoverParams),
+            RequestMethodEnum.COMPLETION: (self._workspace_route, CompletionParams),
+            RequestMethodEnum.CODE_ACTION: (self._workspace_route, CodeActionParams),
         }
 
         self.__notification_mapping = {
             RequestMethodEnum.INITIALIZED: (self._initialized, InitializedParams),
             RequestMethodEnum.CANCEL_REQUEST: (self._cancel_request, CancelParams),
             RequestMethodEnum.PROGRESS: (self._progress, ProgressParams),
             RequestMethodEnum.LOG_TRACE: (self._log_trace, LogTraceParams),
@@ -586,14 +590,24 @@
             rename_provider=RenameOptions(
                 prepare_provider=True,
             ),
             execute_command_provider=ExecuteCommandOptions(
                 commands=[command for command in CommandsEnum]
             ),
             hover_provider=True,
+            completion_provider=CompletionOptions(
+                trigger_characters=[".", '"', "'"],
+                all_commit_characters=None,
+                resolve_provider=None,
+                completion_item=None,
+            ),
+            code_action_provider=CodeActionOptions(
+                code_action_kinds=None,
+                resolve_provider=False,
+            ),
         )
         return InitializeResult(capabilities=server_capabilities, server_info=None)
 
     async def _cancel_request(self, params: CancelParams) -> None:
         if params.id in self.__request_tasks:
             self.__request_tasks[params.id].cancel()
             del self.__request_tasks[params.id]
@@ -814,14 +828,18 @@
             return await self._text_document_will_save(context, params)
         elif isinstance(params, DidSaveTextDocumentParams):
             return await self._text_document_did_save(context, params)
         elif isinstance(params, DidCloseTextDocumentParams):
             return await self._text_document_did_close(context, params)
         elif isinstance(params, HoverParams):
             return await hover(context, params)
+        elif isinstance(params, CompletionParams):
+            return await completion(context, params)
+        elif isinstance(params, CodeActionParams):
+            return await code_action(context, params)
         else:
             raise NotImplementedError(f"Unhandled request: {type(params)}")
 
     async def _text_document_did_open(self, params: DidOpenTextDocumentParams) -> None:
         path = uri_to_path(params.text_document.uri)
         matching_workspaces = []
         for workspace in self.__workspaces.values():
@@ -836,20 +854,22 @@
             context = LspContext(self, await self._create_config(path.parent), False)
             self.__workspaces[path.parent] = context
             context.run()
         else:
             context = min(matching_workspaces, key=lambda x: len(x[1].parts))[0]
 
         await context.compiler.add_change(params)
+        await context.parser.add_change(params)
 
     @staticmethod
     async def _text_document_did_change(
         context: LspContext, params: DidChangeTextDocumentParams
     ) -> None:
         await context.compiler.add_change(params)
+        await context.parser.add_change(params)
 
     @staticmethod
     async def _text_document_will_save(
         context: LspContext, params: WillSaveTextDocumentParams
     ) -> None:
         pass
 
@@ -859,31 +879,35 @@
     ) -> None:
         pass
 
     async def _text_document_did_close(
         self, context: LspContext, params: DidCloseTextDocumentParams
     ) -> None:
         await context.compiler.add_change(params)
+        await context.parser.add_change(params)
 
         if context != self.__main_workspace:
             path = uri_to_path(params.text_document.uri)
             await context.diagnostics_queue.put((path, set()))
         # TODO: remove the workspace from the dict of workspaces (if not main workspace and no other files are open)
 
     async def _workspace_did_create_files(self, params: CreateFilesParams) -> None:
         assert self.__main_workspace is not None
         await self.__main_workspace.compiler.add_change(params)
+        await self.__main_workspace.parser.add_change(params)
 
     async def _workspace_did_rename_files(self, params: RenameFilesParams) -> None:
         assert self.__main_workspace is not None
         await self.__main_workspace.compiler.add_change(params)
+        await self.__main_workspace.parser.add_change(params)
 
     async def _workspace_did_delete_files(self, params: DeleteFilesParams) -> None:
         assert self.__main_workspace is not None
         await self.__main_workspace.compiler.add_change(params)
+        await self.__main_workspace.parser.add_change(params)
 
     async def _workspace_execute_command(
         self, params: ExecuteCommandParams
     ) -> Optional[Any]:
         command = params.command
         if command == CommandsEnum.LSP_FORCE_RECOMPILE:
             for context in self.__workspaces.values():
```

### Comparing `woke-3.3.0/woke/lsp/server_capabilities.py` & `woke-3.4.0/woke/lsp/server_capabilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from typing import Any, List, Optional, Union
 
-from woke.lsp.common_structures import ExecuteCommandOptions, WorkspaceSymbolOptions
+from woke.lsp.common_structures import (
+    ExecuteCommandOptions,
+    PositionEncodingKind,
+    WorkspaceSymbolOptions,
+)
 from woke.lsp.document_sync import TextDocumentSyncKind, TextDocumentSyncOptions
 from woke.utils import StrEnum
 
+from .features.code_action import CodeActionOptions
 from .features.code_lens import CodeLensOptions
+from .features.completion import CompletionOptions
 from .features.definition import DefinitionOptions
 from .features.document_link import DocumentLinkOptions
 from .features.document_symbol import DocumentSymbolOptions
 from .features.hover import HoverOptions
 from .features.implementation import (
     ImplementationOptions,
     ImplementationRegistrationOptions,
@@ -22,20 +28,14 @@
 from .features.type_hierarchy import (
     TypeHierarchyOptions,
     TypeHierarchyRegistrationOptions,
 )
 from .lsp_data_model import LspModel
 
 
-class PositionEncodingKind(StrEnum):
-    UTF8 = "utf-8"
-    UTF16 = "utf-16"
-    UTF32 = "utf-32"
-
-
 class WorkspaceFoldersServerCapabilities(LspModel):
     supported: Optional[bool] = None
     change_notifications: Optional[Union[str, bool]] = None
 
 
 class FileOperationPatternKind(StrEnum):
     FILE = "file"
@@ -131,20 +131,20 @@
     type_definition_provider: Optional[
         Union[bool, TypeDefinitionOptions, TypeDefinitionRegistrationOptions]
     ] = None
     code_lens_provider: Optional[CodeLensOptions] = None
     rename_provider: Optional[Union[bool, RenameOptions]] = None
     execute_command_provider: Optional[ExecuteCommandOptions] = None
     hover_provider: Optional[Union[bool, HoverOptions]] = None
+    completion_provider: Optional[CompletionOptions] = None
+    code_action_provider: Optional[Union[bool, CodeActionOptions]] = None
     """
-    completion_provider: Optional[CompletionOptions]
     signature_help_provider: Optional[SignatureHelpOptions]
     declaration_provider: Optional[Union[bool, DeclarationOptions, DeclarationRegistrationOptions]]
     document_highlight_provider: Optional[Union[bool, ReferenceOptions]]
-    code_action_provider: Optional[Union[bool, CodeActionOptions]]
     color_provider: Optional[Union[bool, DocumentColorOptions, DocumentColorRegistrationOptions]]
     document_formatting_provider: Optional[Union[bool, DocumentFormattingOptions]]
     document_range_formatting_provider: Optional[Union[bool, DocumentRangeFormattingOptions]]
     document_on_type_formatting_provider: Optional[DocumentOnTypeFormattingOptions]
     folding_range_provider: Optional[Union[bool, FoldingRangeOptions, FoldingRangeRegistrationOptions]]
     selection_range_provider: Optional[Union[bool, SelectionRangeOptions, SelectionRangeRegistrationOptions]]
     linked_editing_range_provider: Optional[Union[bool, LinkedEditingRangeOptions, LinkedEditingRangeRegistrationOptions]]
```

### Comparing `woke-3.3.0/woke/lsp/utils/position.py` & `woke-3.4.0/woke/lsp/utils/position.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/regex_parser/solidity_import.py` & `woke-3.4.0/woke/regex_parser/solidity_import.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/regex_parser/solidity_parser.py` & `woke-3.4.0/woke/regex_parser/solidity_parser.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/svm/abc.py` & `woke-3.4.0/woke/svm/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     @abstractmethod
     def list_all(self) -> Tuple[VersionAbc]:
         """
         Return a set of all supported compiler versions.
         :return set of all supported compiler versions
         """
 
-    def list_installed(self) -> Tuple[VersionAbc]:
+    def list_installed(self) -> Tuple[VersionAbc, ...]:
         """
         Return a set of installed compiler versions.
         :return: set of installed compiler versions
         """
         return tuple(version for version in self.list_all() if self.installed(version))
```

### Comparing `woke-3.3.0/woke/svm/svm.py` & `woke-3.4.0/woke/svm/svm.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         dirname = filename
         if dirname.endswith((".exe", ".zip")):
             dirname = dirname[:-4]
         if filename.endswith(".zip"):
             filename = filename[:-3] + "exe"
         return self.__compilers_path / dirname / filename
 
-    def list_all(self) -> Tuple[SolidityVersion]:
+    def list_all(self) -> Tuple[SolidityVersion, ...]:
         self.__fetch_list_file()
         if self.__solc_builds is None:
             raise RuntimeError(
                 f"Unable to fetch or correctly parse '{self.__solc_list_url}'."
             )
 
         return tuple(sorted(self.__solc_builds.releases.keys()))
```

### Comparing `woke-3.3.0/woke/testing/__init__.py` & `woke-3.4.0/woke/testing/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Panic,
     PanicCodeEnum,
     TransactionAbc,
     TransactionRevertedError,
     UnknownTransactionRevertedError,
     may_revert,
     must_revert,
+    on_revert,
 )
 from woke.development.utils import (
     get_create2_address_from_code,
     get_create2_address_from_hash,
     get_create_address,
     keccak256,
 )
```

### Comparing `woke-3.3.0/woke/testing/core.py` & `woke-3.4.0/woke/testing/core.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/testing/coverage.py` & `woke-3.4.0/woke/testing/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     ignore = False
 
     for i, opcode in enumerate(opcodes_spl):
         if ignore:
             ignore = False
             continue
 
-        if not opcode.startswith("PUSH"):
+        if not opcode.startswith("PUSH") or opcode == "PUSH0":
             pc_op_map.append((pc, opcode, 1, None))
             pc += 1
         else:
             size = int(opcode[4:]) + 1
             pc_op_map.append((pc, opcode, size, int(opcodes_spl[i + 1], 16)))
             pc += size
             ignore = True
```

### Comparing `woke-3.3.0/woke/testing/fuzzing/fuzz_test.py` & `woke-3.4.0/woke/testing/fuzzing/fuzz_test.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/testing/fuzzing/fuzzer.py` & `woke-3.4.0/woke/testing/fuzzing/fuzzer.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/testing/fuzzing/generators.py` & `woke-3.4.0/woke/testing/fuzzing/generators.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/utils/context_managers.py` & `woke-3.4.0/woke/utils/context_managers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from contextlib import contextmanager
 from os import chdir
 from pathlib import Path
-from typing import Union, Set
+from typing import Set, Union
 
 
 @contextmanager
 def change_cwd(path: Union[str, Path]):
     """
     Temporary change the current working directory to the path provided as the first argument.
     """
```

### Comparing `woke-3.3.0/woke/utils/decorators.py` & `woke-3.4.0/woke/utils/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from functools import wraps
+
 from .context_managers import recursion_guard
 
 
 def return_on_recursion(default):
     arguments = set()
 
     def decorator(func):
-
         @wraps(func)
         def wrapper(*args, **kwargs):
             if len(kwargs) > 0:
                 raise ValueError("kwargs not supported")
             if args in arguments:
                 return default
             with recursion_guard(arguments, *args):
                 return func(*args, **kwargs)
+
         return wrapper
+
     return decorator
```

### Comparing `woke-3.3.0/woke/utils/file_utils.py` & `woke-3.4.0/woke/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/utils/openzeppelin.py` & `woke-3.4.0/woke/utils/openzeppelin.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/utils/string.py` & `woke-3.4.0/woke/utils/string.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/woke/utils/tee.py` & `woke-3.4.0/woke/utils/tee.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,20 +17,20 @@
         pass
 
     @abstractmethod
     def get_stream(self):
         pass
 
     def write(self, message):
-        self.stream.write(message)  # pyright: reportGeneralTypeIssues=false
-        self.fp.write(message)  # pyright: reportOptionalMemberAccess=false
+        self.stream.write(message)  # pyright: ignore reportGeneralTypeIssues
+        self.fp.write(message)  # pyright: ignore reportOptionalMemberAccess
 
     def flush(self):
-        self.stream.flush()  # pyright: reportGeneralTypeIssues=false
-        self.fp.flush()  # pyright: reportOptionalMemberAccess=false
+        self.stream.flush()  # pyright: ignore reportGeneralTypeIssues
+        self.fp.flush()  # pyright: ignore reportOptionalMemberAccess
 
     def __enter__(self):
         self.stream = self.get_stream()
         self.fp = open(self.filename, self.mode)
         self.set_stream(self)
 
     def __exit__(self, *args):
@@ -45,15 +45,15 @@
             self.stream = None
 
         if self.fp is not None:
             self.fp.close()
             self.fp = None
 
     def isatty(self):
-        return self.stream.isatty()  # pyright: reportGeneralTypeIssues=false
+        return self.stream.isatty()  # pyright: ignore reportGeneralTypeIssues
 
     def __repr__(self):
         return "<%s: %s>" % (self.__class__.__name__, self.filename)
 
     __str__ = __repr__
     __unicode__ = __repr__
```

### Comparing `woke-3.3.0/woke/utils/threaded_child_watcher.py` & `woke-3.4.0/woke/utils/threaded_child_watcher.py`

 * *Files identical despite different names*

### Comparing `woke-3.3.0/setup.py` & `woke-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
  'woke.testing.fuzzing',
  'woke.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiofiles>=0.8,<0.9',
+['abch_tree_sitter>=1.1.1,<2.0.0',
+ 'abch_tree_sitter_solidity>=1.2.0,<2.0.0',
+ 'aiofiles>=0.8,<0.9',
  'aiohttp>=3.8,<4.0',
  'click>=8,<9',
  'eth-abi>=4.0.0b2,<5.0.0',
  'eth-account>=0.8,<0.9',
  'eth-hash[pycryptodome]>=0.5.1,<0.6.0',
  'eth-utils>=2.1,<3.0',
  'graphviz>=0.19,<0.20',
@@ -78,17 +80,17 @@
 
 entry_points = \
 {'console_scripts': ['woke = woke.cli.__main__:main',
                      'woke-solc = woke.cli.__main__:woke_solc']}
 
 setup_kwargs = {
     'name': 'woke',
-    'version': '3.3.0',
+    'version': '3.4.0',
     'description': 'Woke is a Python-based development and testing framework for Solidity.',
-    'long_description': '# Woke\n\nWoke is a Python-based development and testing framework for Solidity.\n\nFeatures:\n\n- **Testing framework** - a testing framework for Solidity smart contracts with Python-native equivalents of Solidity types and blazing fast execution.\n\n- **Fuzzer** - a property-based fuzzer for Solidity smart contracts that allows testers to write their fuzz tests in Python.\n\n- **Vulnerability detectors**\n\n- **LSP server**\n\n## Dependencies\n\n- [Python](https://www.python.org/downloads/release/python-3910/) (version 3.7 or higher)\n\n> :warning: Python 3.11 is experimentally supported.\n\n## Installation\n\nvia `pip`\n\n```shell\npip3 install woke\n```\n\n## Documentation & Contribution\n\nWoke documentation can be found [here](https://ackeeblockchain.com/woke/docs/latest).\n\nThere you can also find a section on [contributing](https://ackeeblockchain.com/woke/docs/latest/contributing/).\n\n## Features\n\n### Testing framework\n\nSee [examples](examples/testing) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.\n\nWriting tests is as simple as:\n\n```python\nfrom woke.testing import *\nfrom pytypes.contracts.Counter import Counter\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n\n    counter = Counter.deploy()\n    assert counter.count() == 0\n\n    counter.increment()\n    assert counter.count() == 1\n```\n\n### Fuzzer\n\nFuzzer builds on top of the testing framework and allows efficient fuzz testing of Solidity smart contracts.\n\n```python\nfrom woke.testing import *\nfrom woke.testing.fuzzing import *\nfrom pytypes.contracts.Counter import Counter\n\nclass CounterTest(FuzzTest):\n    def pre_sequence(self) -> None:\n        self.counter = Counter.deploy()\n        self.count = 0\n\n    @flow()\n    def increment(self) -> None:\n        self.counter.increment()\n        self.count += 1\n\n    @flow()\n    def decrement(self) -> None:\n        with may_revert(Panic(PanicCodeEnum.UNDERFLOW_OVERFLOW)) as e:\n            self.counter.decrement()\n\n        if e.value is not None:\n            assert self.count == 0\n        else:\n            self.count -= 1\n\n    @invariant(period=10)\n    def count(self) -> None:\n        assert self.counter.count() == self.count\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n    CounterTest().run(sequences_count=30, flows_count=100)\n```\n\n### Vulnerability detectors\n\nVulnerability detectors can be run using:\n```shell\nwoke detect\n```\n\n### LSP server\n\nWoke implements an [LSP](https://microsoft.github.io/language-server-protocol/) server for Solidity. The only currently supported communication channel is TCP.\n\nWoke LSP server can be run using:\n\n```shell\nwoke lsp\n```\n\nOr with an optional --port argument:\n\n```shell\nwoke lsp --port 1234\n```\n\nAll LSP server features can be found in the [documentation](https://ackeeblockchain.com/woke/docs/latest/language-server/).\n\n## License\n\nThis project is licensed under the [ISC license](https://github.com/Ackee-Blockchain/woke/blob/main/LICENSE).\n\n## Partners\n\nRockawayX             |  Coinbase\n:-------------------------:|:-------------------------:\n[![](https://github.com/Ackee-Blockchain/woke/blob/main/images/rockawayx.jpg?raw=true)](https://rockawayx.com/)  |  [![](https://github.com/Ackee-Blockchain/woke/blob/main/images/coinbase.png?raw=true)](https://www.coinbase.com/)\n\n\n\n\n\n\n',
+    'long_description': '# Woke\n\nWoke is a Python-based development and testing framework for Solidity.\n\nFeatures:\n\n- **Testing framework** - a testing framework for Solidity smart contracts with Python-native equivalents of Solidity types and blazing fast execution.\n\n- **Fuzzer** - a property-based fuzzer for Solidity smart contracts that allows testers to write their fuzz tests in Python.\n\n- **Vulnerability detectors**\n\n- **LSP server**\n\n## Dependencies\n\n- [Python](https://www.python.org/downloads/release/python-3910/) (version 3.7 or higher)\n\n> :warning: Python 3.11 is experimentally supported.\n\n## Installation\n\nvia `pip`\n\n```shell\npip3 install woke\n```\n\n## Documentation & Contribution\n\nWoke documentation can be found [here](https://ackeeblockchain.com/woke/docs/latest).\n\nThere you can also find a section on [contributing](https://ackeeblockchain.com/woke/docs/latest/contributing/).\n\n## Features\n\n### Testing framework\n\nSee [examples](examples) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.\n\nWriting tests is as simple as:\n\n```python\nfrom woke.testing import *\nfrom pytypes.contracts.Counter import Counter\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n\n    counter = Counter.deploy()\n    assert counter.count() == 0\n\n    counter.increment()\n    assert counter.count() == 1\n```\n\n### Fuzzer\n\nFuzzer builds on top of the testing framework and allows efficient fuzz testing of Solidity smart contracts.\n\n```python\nfrom woke.testing import *\nfrom woke.testing.fuzzing import *\nfrom pytypes.contracts.Counter import Counter\n\nclass CounterTest(FuzzTest):\n    def pre_sequence(self) -> None:\n        self.counter = Counter.deploy()\n        self.count = 0\n\n    @flow()\n    def increment(self) -> None:\n        self.counter.increment()\n        self.count += 1\n\n    @flow()\n    def decrement(self) -> None:\n        with may_revert(Panic(PanicCodeEnum.UNDERFLOW_OVERFLOW)) as e:\n            self.counter.decrement()\n\n        if e.value is not None:\n            assert self.count == 0\n        else:\n            self.count -= 1\n\n    @invariant(period=10)\n    def count(self) -> None:\n        assert self.counter.count() == self.count\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n    CounterTest().run(sequences_count=30, flows_count=100)\n```\n\n### Vulnerability detectors\n\nVulnerability detectors can be run using:\n```shell\nwoke detect\n```\n\n### LSP server\n\nWoke implements an [LSP](https://microsoft.github.io/language-server-protocol/) server for Solidity. The only currently supported communication channel is TCP.\n\nWoke LSP server can be run using:\n\n```shell\nwoke lsp\n```\n\nOr with an optional --port argument:\n\n```shell\nwoke lsp --port 1234\n```\n\nAll LSP server features can be found in the [documentation](https://ackeeblockchain.com/woke/docs/latest/language-server/).\n\n## License\n\nThis project is licensed under the [ISC license](https://github.com/Ackee-Blockchain/woke/blob/main/LICENSE).\n\n## Partners\n\nRockawayX             |  Coinbase\n:-------------------------:|:-------------------------:\n[![](https://github.com/Ackee-Blockchain/woke/blob/main/images/rockawayx.jpg?raw=true)](https://rockawayx.com/)  |  [![](https://github.com/Ackee-Blockchain/woke/blob/main/images/coinbase.png?raw=true)](https://www.coinbase.com/)\n\n\n\n\n\n\n',
     'author': 'Ackee Blockchain',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ackeeblockchain.com',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `woke-3.3.0/PKG-INFO` & `woke-3.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woke
-Version: 3.3.0
+Version: 3.4.0
 Summary: Woke is a Python-based development and testing framework for Solidity.
 Home-page: https://ackeeblockchain.com
 License: ISC
 Keywords: ethereum,solidity,security,testing,development,framework,audit
 Author: Ackee Blockchain
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Provides-Extra: tests
 Requires-Dist: GitPython (>=3.1.20,<4.0.0) ; extra == "tests"
+Requires-Dist: abch_tree_sitter (>=1.1.1,<2.0.0)
+Requires-Dist: abch_tree_sitter_solidity (>=1.2.0,<2.0.0)
 Requires-Dist: aiofiles (>=0.8,<0.9)
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: black (>=22,<23) ; extra == "dev"
 Requires-Dist: cairosvg (>=2.7,<3.0) ; extra == "dev"
 Requires-Dist: click (>=8,<9)
 Requires-Dist: eth-abi (>=4.0.0b2,<5.0.0)
 Requires-Dist: eth-account (>=0.8,<0.9)
@@ -88,15 +90,15 @@
 
 There you can also find a section on [contributing](https://ackeeblockchain.com/woke/docs/latest/contributing/).
 
 ## Features
 
 ### Testing framework
 
-See [examples](examples/testing) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.
+See [examples](examples) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.
 
 Writing tests is as simple as:
 
 ```python
 from woke.testing import *
 from pytypes.contracts.Counter import Counter
```

