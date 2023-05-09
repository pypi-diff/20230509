# Comparing `tmp/bacalhau_apiclient-0.3.29.tar.gz` & `tmp/bacalhau_apiclient-1.0.0.tar.gz`

## Comparing `bacalhau_apiclient-0.3.29.tar` & `bacalhau_apiclient-1.0.0.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/.swagger-codegen-ignore
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/requirements.txt
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/setup.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/test-requirements.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/tox.ini
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/.swagger-codegen/VERSION
--rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/__init__.py
--rw-r--r--   0        0        0    25218 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/api_client.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/configuration.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/rest.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/default_api.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/health_api.py
--rw-r--r--   0        0        0    33905 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/job_api.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/misc_api.py
--rw-r--r--   0        0        0    24993 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/utils_api.py
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/__init__.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_execution_state_run_output.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_execution_state_state.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_create_payload_spec.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_spec.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_spec_language_job_context.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_state_state.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_with_info_job.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_with_info_state.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_deal.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_docker.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_engine.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_network.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_publisher.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_resources.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_ofcancel_request_payload.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_ofevents_request_filters.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_oflog_request_payload.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_ofsubmit_request_payload.py
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/build_version_info.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/cancel_request.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/cancel_response.py
--rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/compute_node_info.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/deal.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/engine.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/event_filter_options.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/events_request.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/events_response.py
--rw-r--r--   0        0        0    14210 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/execution_state.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/execution_state_type.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/free_space.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/health_info.py
--rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_cancel_payload.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_create_payload.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_history.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_history_type.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_requester.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_spec_docker.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_spec_language.py
--rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_spec_wasm.py
--rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_state.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_state_type.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_with_info.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/label_selector_requirement.py
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/list_request.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/list_response.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/log_request.py
--rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/logs_payload.py
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/metadata.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/mount_status.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/network.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/network_config.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/node_info.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/node_type.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/peer_addr_info.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/published_result.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/publisher.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/publisher_spec.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/resource_usage_config.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/resource_usage_data.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/results_response.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/run_command_result.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/s3_storage_spec.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/selection_operator.py
--rw-r--r--   0        0        0    15417 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/spec.py
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/state_change_execution_state_type.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/state_change_job_state_type.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/state_request.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/state_response.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/storage_source_type.py
--rw-r--r--   0        0        0    10253 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/storage_spec.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/submit_request.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/submit_response.py
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/verification_result.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/verifier.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/version_request.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/version_response.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfExecutionStateRunOutput.md
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfExecutionStateState.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfJobCreatePayloadSpec.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfJobSpec.md
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfJobSpecLanguageJobContext.md
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfJobSpecWasmEntryModule.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfJobStateState.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfJobWithInfoJob.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfJobWithInfoState.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfLabelSelectorRequirementOperator.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfSpecDeal.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfSpecDocker.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfSpecEngine.md
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfSpecNetwork.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfSpecPublisher.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfSpecResources.md
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfStorageSpecStorageSource.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfcancelRequestPayload.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfeventsRequestFilters.md
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOflogRequestPayload.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/AllOfsubmitRequestPayload.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/BuildVersionInfo.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/CancelRequest.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/CancelResponse.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/ComputeNodeInfo.md
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/Deal.md
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/DefaultApi.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/Engine.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/EventFilterOptions.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/EventsRequest.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/EventsResponse.md
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/ExecutionState.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/ExecutionStateType.md
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/FreeSpace.md
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/HealthApi.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/HealthInfo.md
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/Job.md
--rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobApi.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobCancelPayload.md
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobCreatePayload.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobHistory.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobHistoryType.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobRequester.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobSpecDocker.md
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobSpecLanguage.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobSpecWasm.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobState.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobStateType.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/JobWithInfo.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/LabelSelectorRequirement.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/ListRequest.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/ListResponse.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/LogRequest.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/LogsPayload.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/Metadata.md
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/MiscApi.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/MountStatus.md
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/Network.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/NetworkConfig.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/NodeInfo.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/NodeType.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/PeerAddrInfo.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/PublishedResult.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/Publisher.md
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/PublisherSpec.md
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/ResourceUsageConfig.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/ResourceUsageData.md
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/ResultsResponse.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/RunCommandResult.md
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/S3StorageSpec.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/SelectionOperator.md
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/Spec.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/StateChangeExecutionStateType.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/StateChangeJobStateType.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/StateRequest.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/StateResponse.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/StorageSourceType.md
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/StorageSpec.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/SubmitRequest.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/SubmitResponse.md
--rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/UtilsApi.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/VerificationResult.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/Verifier.md
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/VersionRequest.md
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/docs/VersionResponse.md
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/LICENSE
--rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/pyproject.toml
--rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.29/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/.swagger-codegen-ignore
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/requirements.txt
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/setup.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/test-requirements.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/tox.ini
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/__init__.py
+-rw-r--r--   0        0        0    25217 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/api_client.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/configuration.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/rest.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/default_api.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/health_api.py
+-rw-r--r--   0        0        0    33905 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/job_api.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/misc_api.py
+-rw-r--r--   0        0        0    24993 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/utils_api.py
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/__init__.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_execution_state_run_output.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_execution_state_state.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_create_payload_spec.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_spec.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_spec_language_job_context.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_state_state.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_with_info_job.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_with_info_state.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_deal.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_docker.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_engine.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_network.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_publisher.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_resources.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_ofcancel_request_payload.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_ofevents_request_filters.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_oflog_request_payload.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_ofsubmit_request_payload.py
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/build_version_info.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/cancel_request.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/cancel_response.py
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/compute_node_info.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/deal.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/engine.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/event_filter_options.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/events_request.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/events_response.py
+-rw-r--r--   0        0        0    14210 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/execution_state.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/execution_state_type.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/free_space.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/health_info.py
+-rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_cancel_payload.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_create_payload.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_history.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_history_type.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_requester.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_spec_docker.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_spec_language.py
+-rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_spec_wasm.py
+-rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_state.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_state_type.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_with_info.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/label_selector_requirement.py
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/list_request.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/list_response.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/log_request.py
+-rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/logs_payload.py
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/metadata.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/mount_status.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/network.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/network_config.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/node_info.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/node_type.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/peer_addr_info.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/published_result.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/publisher.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/publisher_spec.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/resource_usage_config.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/resource_usage_data.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/results_response.py
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/run_command_result.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/s3_storage_spec.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/selection_operator.py
+-rw-r--r--   0        0        0    15417 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/spec.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/state_change_execution_state_type.py
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/state_change_job_state_type.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/state_request.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/state_response.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/storage_source_type.py
+-rw-r--r--   0        0        0    10253 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/storage_spec.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/submit_request.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/submit_response.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/verification_result.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/verifier.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/version_request.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/version_response.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfExecutionStateRunOutput.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfExecutionStateState.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfJobCreatePayloadSpec.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfJobSpec.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfJobSpecLanguageJobContext.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfJobSpecWasmEntryModule.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfJobStateState.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfJobWithInfoJob.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfJobWithInfoState.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfLabelSelectorRequirementOperator.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfSpecDeal.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfSpecDocker.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfSpecEngine.md
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfSpecNetwork.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfSpecPublisher.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfSpecResources.md
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfStorageSpecStorageSource.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfcancelRequestPayload.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfeventsRequestFilters.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOflogRequestPayload.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/AllOfsubmitRequestPayload.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/BuildVersionInfo.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/CancelRequest.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/CancelResponse.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/ComputeNodeInfo.md
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/Deal.md
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/DefaultApi.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/Engine.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/EventFilterOptions.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/EventsRequest.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/EventsResponse.md
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/ExecutionState.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/ExecutionStateType.md
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/FreeSpace.md
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/HealthApi.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/HealthInfo.md
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/Job.md
+-rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobApi.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobCancelPayload.md
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobCreatePayload.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobHistory.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobHistoryType.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobRequester.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobSpecDocker.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobSpecLanguage.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobSpecWasm.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobState.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobStateType.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/JobWithInfo.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/LabelSelectorRequirement.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/ListRequest.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/ListResponse.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/LogRequest.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/LogsPayload.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/Metadata.md
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/MiscApi.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/MountStatus.md
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/Network.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/NetworkConfig.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/NodeInfo.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/NodeType.md
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/PeerAddrInfo.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/PublishedResult.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/Publisher.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/PublisherSpec.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/ResourceUsageConfig.md
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/ResourceUsageData.md
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/ResultsResponse.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/RunCommandResult.md
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/S3StorageSpec.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/SelectionOperator.md
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/Spec.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/StateChangeExecutionStateType.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/StateChangeJobStateType.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/StateRequest.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/StateResponse.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/StorageSourceType.md
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/StorageSpec.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/SubmitRequest.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/SubmitResponse.md
+-rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/UtilsApi.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/VerificationResult.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/Verifier.md
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/VersionRequest.md
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/docs/VersionResponse.md
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.0/PKG-INFO
```

### Comparing `bacalhau_apiclient-0.3.29/.swagger-codegen-ignore` & `bacalhau_apiclient-1.0.0/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/setup.py` & `bacalhau_apiclient-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: team@bacalhau.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "bacalhau_apiclient"
-VERSION = "0.3.29"
+VERSION = "1.0.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/__init__.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/api_client.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/0.3.29/python'
+        self.user_agent = 'Swagger-Codegen/1.0.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/configuration.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,9 +236,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: ${PYPI_VERSION}\n"\
-               "SDK Package Version: 0.3.29".\
+               "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/rest.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/rest.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/default_api.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/default_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/health_api.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/health_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/job_api.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/job_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/misc_api.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/misc_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/api/utils_api.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/__init__.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_execution_state_run_output.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_execution_state_run_output.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_execution_state_state.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_execution_state_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_create_payload_spec.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_create_payload_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_spec.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_spec_language_job_context.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_spec_language_job_context.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_state_state.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_state_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_with_info_job.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_with_info_job.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_job_with_info_state.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_job_with_info_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_deal.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_deal.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_docker.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_docker.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_engine.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_engine.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_network.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_network.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_publisher.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_publisher.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_spec_resources.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_spec_resources.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_ofcancel_request_payload.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_ofcancel_request_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_ofevents_request_filters.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_ofevents_request_filters.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_oflog_request_payload.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_oflog_request_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/all_ofsubmit_request_payload.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/all_ofsubmit_request_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/build_version_info.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/build_version_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/cancel_request.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/cancel_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/cancel_response.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/cancel_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/compute_node_info.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/compute_node_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/deal.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/deal.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/engine.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/engine.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/event_filter_options.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/event_filter_options.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/events_request.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/events_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/events_response.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/events_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/execution_state.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/execution_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/execution_state_type.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/execution_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/free_space.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/free_space.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/health_info.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/health_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_cancel_payload.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_cancel_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_create_payload.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_create_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_history.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_history.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_history_type.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_history_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_requester.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_requester.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_spec_docker.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_spec_docker.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_spec_language.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_spec_language.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_spec_wasm.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_spec_wasm.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_state.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_state_type.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/job_with_info.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/job_with_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/label_selector_requirement.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/label_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/list_request.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/list_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/list_response.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/list_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/log_request.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/log_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/logs_payload.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/logs_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/metadata.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/metadata.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/mount_status.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/mount_status.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/network.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/network.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/network_config.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/network_config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/node_info.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/node_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/node_type.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/node_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/peer_addr_info.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/peer_addr_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/published_result.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/published_result.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/publisher.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/publisher.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/publisher_spec.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/publisher_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/resource_usage_config.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/resource_usage_config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/resource_usage_data.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/resource_usage_data.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/results_response.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/results_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/run_command_result.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/run_command_result.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/s3_storage_spec.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/s3_storage_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/selection_operator.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/selection_operator.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/spec.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/state_change_execution_state_type.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/state_change_execution_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/state_change_job_state_type.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/state_change_job_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/state_request.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/state_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/state_response.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/state_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/storage_source_type.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/storage_source_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/storage_spec.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/storage_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/submit_request.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/submit_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/submit_response.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/submit_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/verification_result.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/verification_result.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/verifier.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/verifier.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/version_request.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/version_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/bacalhau_apiclient/models/version_response.py` & `bacalhau_apiclient-1.0.0/bacalhau_apiclient/models/version_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/BuildVersionInfo.md` & `bacalhau_apiclient-1.0.0/docs/BuildVersionInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/CancelRequest.md` & `bacalhau_apiclient-1.0.0/docs/CancelRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/ComputeNodeInfo.md` & `bacalhau_apiclient-1.0.0/docs/ComputeNodeInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/Deal.md` & `bacalhau_apiclient-1.0.0/docs/Deal.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/DefaultApi.md` & `bacalhau_apiclient-1.0.0/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/ExecutionState.md` & `bacalhau_apiclient-1.0.0/docs/ExecutionState.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/HealthApi.md` & `bacalhau_apiclient-1.0.0/docs/HealthApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/JobApi.md` & `bacalhau_apiclient-1.0.0/docs/JobApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/JobCancelPayload.md` & `bacalhau_apiclient-1.0.0/docs/JobCancelPayload.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/JobHistory.md` & `bacalhau_apiclient-1.0.0/docs/JobHistory.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/JobRequester.md` & `bacalhau_apiclient-1.0.0/docs/JobRequester.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/JobSpecDocker.md` & `bacalhau_apiclient-1.0.0/docs/JobSpecDocker.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/JobSpecLanguage.md` & `bacalhau_apiclient-1.0.0/docs/JobSpecLanguage.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/JobSpecWasm.md` & `bacalhau_apiclient-1.0.0/docs/JobSpecWasm.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/JobState.md` & `bacalhau_apiclient-1.0.0/docs/JobState.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/JobWithInfo.md` & `bacalhau_apiclient-1.0.0/docs/JobWithInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/LabelSelectorRequirement.md` & `bacalhau_apiclient-1.0.0/docs/LabelSelectorRequirement.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/ListRequest.md` & `bacalhau_apiclient-1.0.0/docs/ListRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/LogRequest.md` & `bacalhau_apiclient-1.0.0/docs/LogRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/LogsPayload.md` & `bacalhau_apiclient-1.0.0/docs/LogsPayload.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/Metadata.md` & `bacalhau_apiclient-1.0.0/docs/Metadata.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/MiscApi.md` & `bacalhau_apiclient-1.0.0/docs/MiscApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/NodeInfo.md` & `bacalhau_apiclient-1.0.0/docs/NodeInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/ResourceUsageConfig.md` & `bacalhau_apiclient-1.0.0/docs/ResourceUsageConfig.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/RunCommandResult.md` & `bacalhau_apiclient-1.0.0/docs/RunCommandResult.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/S3StorageSpec.md` & `bacalhau_apiclient-1.0.0/docs/S3StorageSpec.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/Spec.md` & `bacalhau_apiclient-1.0.0/docs/Spec.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/StorageSpec.md` & `bacalhau_apiclient-1.0.0/docs/StorageSpec.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/SubmitRequest.md` & `bacalhau_apiclient-1.0.0/docs/SubmitRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/docs/UtilsApi.md` & `bacalhau_apiclient-1.0.0/docs/UtilsApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/.gitignore` & `bacalhau_apiclient-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/LICENSE` & `bacalhau_apiclient-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.29/README.md` & `bacalhau_apiclient-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # bacalhau_apiclient
 This page is the reference of the Bacalhau REST API. Project docs are available at https://docs.bacalhau.org/. Find more information about Bacalhau at https://github.com/bacalhau-project/bacalhau.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: ${PYPI_VERSION}
-- Package version: 0.3.29
+- Package version: 1.0.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 For more information, please visit [https://github.com/bacalhau-project/bacalhau](https://github.com/bacalhau-project/bacalhau)
 
 ## Requirements.
 
 Python 3.6+
```

### Comparing `bacalhau_apiclient-0.3.29/pyproject.toml` & `bacalhau_apiclient-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bacalhau_apiclient"
-version = "0.3.29"
+version = "1.0.0"
 authors = [
 { name="Enrico Rotundo", email="enrico.rotundo@gmail.com" },
 ]
 description = "A Python client for the Bacalhau public API - https://github.com/bacalhau-project/bacalhau/tree/main/clients/python"
 readme = "README.md"
 requires-python = ">=3.6.2"
 classifiers = [
```

### Comparing `bacalhau_apiclient-0.3.29/PKG-INFO` & `bacalhau_apiclient-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau_apiclient
-Version: 0.3.29
+Version: 1.0.0
 Summary: A Python client for the Bacalhau public API - https://github.com/bacalhau-project/bacalhau/tree/main/clients/python
 Project-URL: Homepage, https://github.com/bacalhau-project/bacalhau/
 Project-URL: Bug Tracker, https://github.com/bacalhau-project/bacalhau/issues
 Author-email: Enrico Rotundo <enrico.rotundo@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 
 # bacalhau_apiclient
 This page is the reference of the Bacalhau REST API. Project docs are available at https://docs.bacalhau.org/. Find more information about Bacalhau at https://github.com/bacalhau-project/bacalhau.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: ${PYPI_VERSION}
-- Package version: 0.3.29
+- Package version: 1.0.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 For more information, please visit [https://github.com/bacalhau-project/bacalhau](https://github.com/bacalhau-project/bacalhau)
 
 ## Requirements.
 
 Python 3.6+
```

