# Comparing `tmp/tuf-2.1.0.tar.gz` & `tmp/tuf-3.0.0.tar.gz`

## Comparing `tuf-2.1.0.tar` & `tuf-3.0.0.tar`

### file list

```diff
@@ -1,190 +1,194 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 tuf-2.1.0/requirements-build.txt
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 tuf-2.1.0/requirements-dev.txt
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tuf-2.1.0/requirements-docs.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 tuf-2.1.0/requirements-pinned.txt
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 tuf-2.1.0/requirements-test.txt
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tuf-2.1.0/requirements.txt
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 tuf-2.1.0/tox.ini
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/1.0.0-ANNOUNCEMENT.md
--rw-r--r--   0        0        0    28556 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/CONTRIBUTING.rst
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/GOVERNANCE.md
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/INSTALLATION.rst
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/MAINTAINERS.txt
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/RELEASE.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/SECURITY.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/_config.yml
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/conf.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/index.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/index.rst
--rw-r--r--   0        0        0    50177 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/repository-library-design-ownership.jpg
--rw-r--r--   0        0        0    42997 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/repository-library-design-usage.jpg
--rw-r--r--   0        0        0    11688 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/repository-library-design.md
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/tuf-horizontal-white.png
--rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/tuf-icon-200.png
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/tuf-icon-32.png
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/_posts/2022-02-21-release-1-0-0.md
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/_posts/2022-05-04-ngclient-design.md
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/_posts/2022-06-15-testing-ngclient.md
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0000-use-markdown-architectural-decision-records.md
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0001-python-version-3-6-plus.md
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0002-pre-1-0-deprecation-strategy.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0005-use-google-python-style-guide.md
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0006-where-to-implemenent-model-serialization.md
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0008-accept-unrecognised-fields.md
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0009-what-is-a-reference-implementation.md
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/0010-repository-library-design.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/index.md
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/adr/template.md
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/api-reference.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.api.metadata.metadata.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.api.metadata.root.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.api.metadata.snapshot.rst
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.api.metadata.supporting.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.api.metadata.targets.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.api.metadata.timestamp.rst
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.api.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.api.serialization.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.ngclient.config.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.ngclient.fetcher.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.ngclient.rst
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tuf-2.1.0/docs/api/tuf.ngclient.updater.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 tuf-2.1.0/examples/README.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tuf-2.1.0/examples/client_example/README.md
--rwxr-xr-x   0        0        0     4850 2020-02-02 00:00:00.000000 tuf-2.1.0/examples/client_example/client
--rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 tuf-2.1.0/examples/manual_repo/basic_repo.py
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 tuf-2.1.0/examples/manual_repo/hashed_bin_delegation.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 tuf-2.1.0/examples/manual_repo/succinct_hash_bin_delegations.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tuf-2.1.0/examples/repository/README.md
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 tuf-2.1.0/examples/repository/_simplerepo.py
--rwxr-xr-x   0        0        0     3605 2020-02-02 00:00:00.000000 tuf-2.1.0/examples/repository/repo
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/.coveragerc
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/__init__.py
--rwxr-xr-x   0        0        0      904 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/aggregate_tests.py
--rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_simulator.py
--rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/simple_server.py
--rwxr-xr-x   0        0        0    32782 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_api.py
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_examples.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_fetcher_ng.py
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_metadata_eq_.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_metadata_generation.py
--rw-r--r--   0        0        0    33649 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_metadata_serialization.py
--rw-r--r--   0        0        0    20169 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_trusted_metadata_set.py
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_updater_consistent_snapshot.py
--rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_updater_delegation_graphs.py
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_updater_fetch_target.py
--rw-r--r--   0        0        0    12164 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_updater_key_rotations.py
--rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_updater_ng.py
--rw-r--r--   0        0        0    31512 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_updater_top_level_update.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_updater_validation.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/test_utils.py
--rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/generated_data/__init__.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/generated_data/generate_md.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/generated_data/ed25519_metadata/snapshot_with_ed25519.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/generated_data/ed25519_metadata/targets_with_ed25519.json
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/generated_data/ed25519_metadata/timestamp_with_ed25519.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/README.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/map.json
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/map.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/fishy_rolenames/1.a.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/fishy_rolenames/metadata/1...json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/fishy_rolenames/metadata/1.root.json
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/fishy_rolenames/metadata/1.ö.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/fishy_rolenames/metadata/timestamp.json
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/delegation_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/delegation_key.pub
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/root_key
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/root_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/root_key2
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/root_key2.pub
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/root_key3
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/root_key3.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/snapshot_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/snapshot_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/targets_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/targets_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/timestamp_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/keystore/timestamp_key.pub
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/project/targets/file1.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/project/targets/file2.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/project/targets/file3.txt
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/project/test-flat/project.cfg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/project/test-flat/role1.json
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/project/test-flat/test-flat.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata/role1.json
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata.staged/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata.staged/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata.staged/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata.staged/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata.staged/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata.staged/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/metadata.staged/timestamp.json
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/targets/file1.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/targets/file2.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tuf-2.1.0/tests/repository_data/repository/targets/file3.txt
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/api/__init__.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/api/exceptions.py
--rw-r--r--   0        0        0    75502 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/api/metadata.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/api/serialization/__init__.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/api/serialization/json.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/ngclient/README.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/ngclient/__init__.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/ngclient/config.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/ngclient/fetcher.py
--rw-r--r--   0        0        0    19947 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/ngclient/updater.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/ngclient/_internal/__init__.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/ngclient/_internal/requests_fetcher.py
--rw-r--r--   0        0        0    18775 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/ngclient/_internal/trusted_metadata_set.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/repository/__init__.py
--rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 tuf-2.1.0/tuf/repository/_repository.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-2.1.0/.gitignore
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 tuf-2.1.0/LICENSE
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tuf-2.1.0/LICENSE-MIT
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 tuf-2.1.0/README.md
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 tuf-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 tuf-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 tuf-3.0.0/tox.ini
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/1.0.0-ANNOUNCEMENT.md
+-rw-r--r--   0        0        0    29833 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/GOVERNANCE.md
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/INSTALLATION.rst
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/MAINTAINERS.txt
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/RELEASE.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/SECURITY.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/_config.yml
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/conf.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/index.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/index.rst
+-rw-r--r--   0        0        0    50177 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/repository-library-design-ownership.jpg
+-rw-r--r--   0        0        0    42997 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/repository-library-design-usage.jpg
+-rw-r--r--   0        0        0    11688 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/repository-library-design.md
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/tuf-horizontal-white.png
+-rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/tuf-icon-200.png
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/tuf-icon-32.png
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/_posts/2022-02-21-release-1-0-0.md
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/_posts/2022-05-04-ngclient-design.md
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/_posts/2022-06-15-testing-ngclient.md
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0000-use-markdown-architectural-decision-records.md
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0001-python-version-3-6-plus.md
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0002-pre-1-0-deprecation-strategy.md
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0005-use-google-python-style-guide.md
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0006-where-to-implemenent-model-serialization.md
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0008-accept-unrecognised-fields.md
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0009-what-is-a-reference-implementation.md
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/0010-repository-library-design.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/index.md
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/adr/template.md
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/api-reference.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.api.metadata.metadata.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.api.metadata.root.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.api.metadata.snapshot.rst
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.api.metadata.supporting.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.api.metadata.targets.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.api.metadata.timestamp.rst
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.api.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.api.serialization.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.ngclient.config.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.ngclient.fetcher.rst
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.ngclient.rst
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tuf-3.0.0/docs/api/tuf.ngclient.updater.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/README.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/client/README.md
+-rwxr-xr-x   0        0        0     4850 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/client/client
+-rw-r--r--   0        0        0    14711 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/manual_repo/basic_repo.py
+-rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/manual_repo/hashed_bin_delegation.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/manual_repo/succinct_hash_bin_delegations.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/repository/README.md
+-rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/repository/_simplerepo.py
+-rwxr-xr-x   0        0        0     4484 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/repository/repo
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/uploader/README.md
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/uploader/_localrepo.py
+-rwxr-xr-x   0        0        0     4262 2020-02-02 00:00:00.000000 tuf-3.0.0/examples/uploader/uploader
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 tuf-3.0.0/requirements/build.txt
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tuf-3.0.0/requirements/dev.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tuf-3.0.0/requirements/docs.txt
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 tuf-3.0.0/requirements/lint.txt
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tuf-3.0.0/requirements/main.txt
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 tuf-3.0.0/requirements/pinned.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 tuf-3.0.0/requirements/test.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/.coveragerc
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/__init__.py
+-rwxr-xr-x   0        0        0      904 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/aggregate_tests.py
+-rw-r--r--   0        0        0    15467 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_simulator.py
+-rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/simple_server.py
+-rwxr-xr-x   0        0        0    34243 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_api.py
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_examples.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_fetcher_ng.py
+-rw-r--r--   0        0        0     6999 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_metadata_eq_.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_metadata_generation.py
+-rw-r--r--   0        0        0    33661 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_metadata_serialization.py
+-rw-r--r--   0        0        0    20171 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_trusted_metadata_set.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_updater_consistent_snapshot.py
+-rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_updater_delegation_graphs.py
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_updater_fetch_target.py
+-rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_updater_key_rotations.py
+-rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_updater_ng.py
+-rw-r--r--   0        0        0    31511 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_updater_top_level_update.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_updater_validation.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/generated_data/__init__.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/generated_data/generate_md.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/generated_data/ed25519_metadata/snapshot_with_ed25519.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/generated_data/ed25519_metadata/targets_with_ed25519.json
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/generated_data/ed25519_metadata/timestamp_with_ed25519.json
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/README.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/map.json
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/map.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/fishy_rolenames/1.a.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/fishy_rolenames/metadata/1...json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/fishy_rolenames/metadata/1.root.json
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/fishy_rolenames/metadata/1.ö.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/fishy_rolenames/metadata/timestamp.json
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/delegation_key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/delegation_key.pub
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/root_key
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/root_key.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/root_key2
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/root_key2.pub
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/root_key3
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/root_key3.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/snapshot_key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/snapshot_key.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/targets_key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/targets_key.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/timestamp_key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/keystore/timestamp_key.pub
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/project/targets/file1.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/project/targets/file2.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/project/targets/file3.txt
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/project/test-flat/project.cfg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/project/test-flat/role1.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/project/test-flat/test-flat.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata/role1.json
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata.staged/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata.staged/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata.staged/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata.staged/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata.staged/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata.staged/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/metadata.staged/timestamp.json
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/targets/file1.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/targets/file2.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tuf-3.0.0/tests/repository_data/repository/targets/file3.txt
+-rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/api/__init__.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/api/exceptions.py
+-rw-r--r--   0        0        0    71169 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/api/metadata.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/api/serialization/__init__.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/api/serialization/json.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/ngclient/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/ngclient/__init__.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/ngclient/config.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/ngclient/fetcher.py
+-rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/ngclient/updater.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/ngclient/_internal/__init__.py
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/ngclient/_internal/requests_fetcher.py
+-rw-r--r--   0        0        0    18775 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/ngclient/_internal/trusted_metadata_set.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/repository/__init__.py
+-rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 tuf-3.0.0/tuf/repository/_repository.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-3.0.0/.gitignore
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 tuf-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tuf-3.0.0/LICENSE-MIT
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 tuf-3.0.0/README.md
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 tuf-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 tuf-3.0.0/PKG-INFO
```

### Comparing `tuf-2.1.0/requirements.txt` & `tuf-3.0.0/requirements/main.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # TUF runtime requirements plus securesystemslib with extra dependencies
 #
 # This file together with 'pip-compile' is used to generate a pinned
 # requirements file with all immediate and transitive dependencies.
 #
-# 'requirements-pinned.txt' is updated on GitHub with Dependabot, which
+# 'pinned.txt' is updated on GitHub with Dependabot, which
 # triggers CI/CD builds to automatically test against updated dependencies.
 #
 #
 # NOTE: 'pip-compile' only adds dependencies relevant for the Python version,
 # in which it is executed. Moreover, it does not add environment markers of
 # transitive dependencies.
 # The official recommendation for cross-environment usage of pip-compile tends
 # towards separate requirements files for each environment (see
 # jazzband/pip-tools#651), this seem like an overkill for tuf, where we only
 # have a few conditional dependencies, i.e. dependencies that are required on
 # Python < 3 only.
 #
 #
-# Below instructions can be used to re-generate 'requirements-pinned.txt', e.g.
+# Below instructions can be used to re-generate 'pinned.txt', e.g.
 # if:
 # - requirements are added or removed from this file
 # - Python version support is changed
 # - CI/CD build breaks due to updates (e.g. transitive dependency conflicts)
 #
 # 1. Use this script to create a pinned requirements file for each Python
 #    version
 # ```
 # for v in 3.7 3.8 3.9 3.10 3.11; do
 #   mkvirtualenv tuf-env-${v} -p python${v};
 #   python3 -m pip install pip-tools;
-#   pip-compile --no-header -o requirements-${v}.txt requirements.txt;
+#   pip-compile --no-header -o requirements-${v}.txt main.txt;
 #   deactivate;
 #   rmvirtualenv tuf-env-${v};
 # done;
 #
 # ```
 # 2. Use this command to merge per-version files
-#    `sort -o requirements-pinned.txt -u requirements-?.?.txt`
-# 2. Manually add environment markers to requirements-pinned.txt
+#    `sort -o pinned.txt -u requirements-?.?.txt`
+# 2. Manually add environment markers to pinned.txt
 # 3. Use this command to remove per-version files
 #    `rm requirements-?.?.txt`
 #
 securesystemslib[crypto, pynacl]
 requests
```

### Comparing `tuf-2.1.0/tox.ini` & `tuf-3.0.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -16,46 +16,51 @@
 
 commands =
     python3 --version
     python3 -m coverage run aggregate_tests.py
     python3 -m coverage report -m --fail-under 97
 
 deps =
-    -r{toxinidir}/requirements-test.txt
+    -r{toxinidir}/requirements/test.txt
     # Install TUF in editable mode, instead of tox default virtual environment
     # installation (see `skipsdist`), to get relative paths in coverage reports
     --editable {toxinidir}
 
 install_command = python3 -m pip install {opts} {packages}
 
 # Workaround https://github.com/tox-dev/tox/issues/2801 (python3 not allowed in Windows)
 allowlist_externals = python3
 
-# Develop test env to run tests against securesystemslib's master branch
-# Must to be invoked explicitly with, e.g. `tox -e with-sslib-master`
-[testenv:with-sslib-master]
+# Develop test env to run tests against securesystemslib's main branch
+# Must to be invoked explicitly with, e.g. `tox -e with-sslib-main`
+[testenv:with-sslib-main]
 commands_pre =
-    python3 -m pip install git+https://github.com/secure-systems-lab/securesystemslib.git@master#egg=securesystemslib[crypto,pynacl]
+    python3 -m pip install --force-reinstall git+https://github.com/secure-systems-lab/securesystemslib.git@main#egg=securesystemslib[crypto,pynacl]
 
 commands =
     python3 -m coverage run aggregate_tests.py
     python3 -m coverage report -m
 
 [testenv:lint]
 changedir = {toxinidir}
+deps =
+    -r{toxinidir}/requirements/lint.txt
+    --editable {toxinidir}
 lint_dirs = tuf examples tests verify_release
 commands =
     black --check --diff {[testenv:lint]lint_dirs}
     isort --check --diff {[testenv:lint]lint_dirs}
     pylint -j 0 --rcfile=pyproject.toml {[testenv:lint]lint_dirs}
 
     mypy {[testenv:lint]lint_dirs}
 
     bandit -r tuf
 
+    pydocstyle tuf
+
 [testenv:docs]
 deps =
-    -r{toxinidir}/requirements-docs.txt
+    -r{toxinidir}/requirements/docs.txt
 
 changedir = {toxinidir}
 commands =
     sphinx-build -b html docs docs/build/html -W
```

### Comparing `tuf-2.1.0/docs/1.0.0-ANNOUNCEMENT.md` & `tuf-3.0.0/docs/1.0.0-ANNOUNCEMENT.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/CHANGELOG.md` & `tuf-3.0.0/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,41 @@
 # Changelog
+
+## v3.0.0
+
+The notable change in this release is #2165: The tuf.api.metadata.Key
+class implementation was moved to Securesystemslib with minor API
+changes. These changes require no action in tuf.ngclient users but may
+require small changes in tuf.api.metadata using repository
+implementations that create keys.
+
+As a result of these changes, both signing and verification are now
+fully extensible, see Securesystemslib signer API for details.
+
+tuf.repository remains an unstable module in 3.0.0.
+
+### Added
+* Build: Use pydocstyle to lint docstrings (#2283, #2281)
+* Examples: Add Repository uploader/signer tool example (#2241)
+* Metadata API: Add TargetFile.get_prefixed_paths() (#2166)
+* ngclient: Export TargetFile (#2279)
+* repository: Add strictly typed accessors and context managers (#2311)
+* Release: Use PyPI Trusted Publishing
+  https://docs.pypi.org/trusted-publishers/ (#2371)
+
+### Changed
+* Build: Various minor build and release infrastructure improvements,
+  dependency updates
+* Metadata API: Key class is still part of the API but now comes from
+  Securesystemslib (#2165):
+  * `Key.verify_signature()` method signature has changed
+  * `Key.from_securesystemslib_key()` was removed: Use
+    Securesystemslibs `SSlibKey.from_securesystemslib_key()` instead
+
+
 ## v2.1.0
 ### Added
 * repo: experimental repository module and example (#2193)
 * ngclient: expose default requests fetcher (#2277)
 * workflow: OpenSSF scorecard (#2190)
 * build: Python 3.11 support (#2157)
 * docs: security policy (#2098, #2178)
```

### Comparing `tuf-2.1.0/docs/CONTRIBUTING.rst` & `tuf-3.0.0/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/GOVERNANCE.md` & `tuf-3.0.0/docs/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/INSTALLATION.rst` & `tuf-3.0.0/docs/INSTALLATION.rst`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 .. note::
 
    Development installation will `Install with full cryptographic abilities`_.
    Please check above for possible system dependencies.
 
 ::
 
-   python3 -m pip install -r requirements-dev.txt
+   python3 -m pip install -r requirements/dev.txt
 
 
 Verify release signatures
 -------------------------
 
 Releases on PyPI are signed with a maintainer key using
 `gpg <https://gnupg.org/>`_  (see
```

### Comparing `tuf-2.1.0/docs/MAINTAINERS.txt` & `tuf-3.0.0/docs/MAINTAINERS.txt`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/RELEASE.md` & `tuf-3.0.0/docs/RELEASE.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/SECURITY.md` & `tuf-3.0.0/docs/SECURITY.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/conf.py` & `tuf-3.0.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,16 +57,14 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ['_static']
 
 # -- Autodoc configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
 
-autodoc_mock_imports = ["securesystemslib"]
-
 # Tone down the "tuf.api.metadata." repetition
 add_module_names = False
 python_use_unqualified_type_names = True
 
 # Show typehints in argument doc lines, but not in signatures
 autodoc_typehints = "description"
```

### Comparing `tuf-2.1.0/docs/index.rst` & `tuf-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/repository-library-design-ownership.jpg` & `tuf-3.0.0/docs/repository-library-design-ownership.jpg`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/repository-library-design-usage.jpg` & `tuf-3.0.0/docs/repository-library-design-usage.jpg`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/repository-library-design.md` & `tuf-3.0.0/docs/repository-library-design.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/tuf-horizontal-white.png` & `tuf-3.0.0/docs/tuf-horizontal-white.png`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/tuf-icon-200.png` & `tuf-3.0.0/docs/tuf-icon-200.png`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/tuf-icon-32.png` & `tuf-3.0.0/docs/tuf-icon-32.png`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/_posts/2022-02-21-release-1-0-0.md` & `tuf-3.0.0/docs/_posts/2022-02-21-release-1-0-0.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/_posts/2022-05-04-ngclient-design.md` & `tuf-3.0.0/docs/_posts/2022-05-04-ngclient-design.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/_posts/2022-06-15-testing-ngclient.md` & `tuf-3.0.0/docs/_posts/2022-06-15-testing-ngclient.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md` & `tuf-3.0.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md` & `tuf-3.0.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0000-use-markdown-architectural-decision-records.md` & `tuf-3.0.0/docs/adr/0000-use-markdown-architectural-decision-records.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0001-python-version-3-6-plus.md` & `tuf-3.0.0/docs/adr/0001-python-version-3-6-plus.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0002-pre-1-0-deprecation-strategy.md` & `tuf-3.0.0/docs/adr/0002-pre-1-0-deprecation-strategy.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md` & `tuf-3.0.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md` & `tuf-3.0.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0005-use-google-python-style-guide.md` & `tuf-3.0.0/docs/adr/0005-use-google-python-style-guide.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0006-where-to-implemenent-model-serialization.md` & `tuf-3.0.0/docs/adr/0006-where-to-implemenent-model-serialization.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0008-accept-unrecognised-fields.md` & `tuf-3.0.0/docs/adr/0008-accept-unrecognised-fields.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0009-what-is-a-reference-implementation.md` & `tuf-3.0.0/docs/adr/0009-what-is-a-reference-implementation.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/0010-repository-library-design.md` & `tuf-3.0.0/docs/adr/0010-repository-library-design.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/index.md` & `tuf-3.0.0/docs/adr/index.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/adr/template.md` & `tuf-3.0.0/docs/adr/template.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/api/api-reference.rst` & `tuf-3.0.0/docs/api/api-reference.rst`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/api/tuf.api.metadata.supporting.rst` & `tuf-3.0.0/docs/api/tuf.api.metadata.supporting.rst`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/docs/api/tuf.ngclient.rst` & `tuf-3.0.0/docs/api/tuf.ngclient.rst`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/examples/client_example/README.md` & `tuf-3.0.0/examples/client/README.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/examples/client_example/client` & `tuf-3.0.0/examples/client/client`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,14 @@
 
 
 def init_tofu(base_url: str) -> bool:
     """Initialize local trusted metadata (Trust-On-First-Use) and create a
     directory for downloads"""
     metadata_dir = build_metadata_dir(base_url)
 
-    if not os.path.isdir(DOWNLOAD_DIR):
-        os.mkdir(DOWNLOAD_DIR)
-
     if not os.path.isdir(metadata_dir):
         os.makedirs(metadata_dir)
 
     root_url = f"{base_url}/metadata/1.root.json"
     try:
         request.urlretrieve(root_url, f"{metadata_dir}/root.json")
     except OSError:
@@ -68,14 +65,17 @@
             "Trust-On-First-Use or copy trusted root metadata to "
             f"{metadata_dir}/root.json"
         )
         return False
 
     print(f"Using trusted root in {metadata_dir}")
 
+    if not os.path.isdir(DOWNLOAD_DIR):
+        os.mkdir(DOWNLOAD_DIR)
+
     try:
         updater = Updater(
             metadata_dir=metadata_dir,
             metadata_base_url=f"{base_url}/metadata/",
             target_base_url=f"{base_url}/targets/",
             target_dir=DOWNLOAD_DIR,
         )
```

### Comparing `tuf-2.1.0/examples/manual_repo/basic_repo.py` & `tuf-3.0.0/examples/manual_repo/basic_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,20 @@
 import os
 import tempfile
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Any, Dict
 
 from securesystemslib.keys import generate_ed25519_key
-from securesystemslib.signer import SSlibSigner
+from securesystemslib.signer import SSlibKey, SSlibSigner
 
 from tuf.api.metadata import (
     SPECIFICATION_VERSION,
     DelegatedRole,
     Delegations,
-    Key,
     Metadata,
     MetaFile,
     Root,
     Snapshot,
     TargetFile,
     Targets,
     Timestamp,
@@ -153,15 +152,15 @@
 # For this example, we generate one 'ed25519' key pair for each top-level role
 # using python-tuf's in-house crypto library.
 # See https://github.com/secure-systems-lab/securesystemslib for more details
 # about key handling, and don't forget to password-encrypt your private keys!
 for name in ["targets", "snapshot", "timestamp", "root"]:
     keys[name] = generate_ed25519_key()
     roles["root"].signed.add_key(
-        Key.from_securesystemslib_key(keys[name]), name
+        SSlibKey.from_securesystemslib_key(keys[name]), name
     )
 
 # NOTE: We only need the public part to populate root, so it is possible to use
 # out-of-band mechanisms to generate key pairs and only expose the public part
 # to whoever maintains the root role. As a matter of fact, the very purpose of
 # signature thresholds is to avoid having private keys all in one place.
 
@@ -169,15 +168,15 @@
 # --------------------
 # Given the importance of the root role, it is highly recommended to require a
 # threshold of multiple keys to sign root metadata. For this example we
 # generate another root key (you can pretend it's out-of-band) and increase the
 # required signature threshold.
 another_root_key = generate_ed25519_key()
 roles["root"].signed.add_key(
-    Key.from_securesystemslib_key(another_root_key), "root"
+    SSlibKey.from_securesystemslib_key(another_root_key), "root"
 )
 roles["root"].signed.roles["root"].threshold = 2
 
 
 # Sign top-level metadata (in-band)
 # =================================
 # In this example we have access to all top-level signing keys, so we can use
@@ -267,15 +266,15 @@
 # The delegation info defined by the delegator further requires the provision
 # of a unique delegatee name and constraints about the target files the
 # delegatee is responsible for, e.g. a list of path patterns. For details about
 # all configuration parameters see
 # https://theupdateframework.github.io/specification/latest/#delegations
 roles["targets"].signed.delegations = Delegations(
     keys={
-        keys[delegatee_name]["keyid"]: Key.from_securesystemslib_key(
+        keys[delegatee_name]["keyid"]: SSlibKey.from_securesystemslib_key(
             keys[delegatee_name]
         )
     },
     roles={
         delegatee_name: DelegatedRole(
             name=delegatee_name,
             keyids=[keys[delegatee_name]["keyid"]],
@@ -341,15 +340,15 @@
 # In this example we will replace a root key, and sign a new version of root
 # with the threshold of old and new keys. Since one of the previous root keys
 # remains in place, it can be used to count towards the old and new threshold.
 new_root_key = generate_ed25519_key()
 
 roles["root"].signed.revoke_key(keys["root"]["keyid"], "root")
 roles["root"].signed.add_key(
-    Key.from_securesystemslib_key(new_root_key), "root"
+    SSlibKey.from_securesystemslib_key(new_root_key), "root"
 )
 roles["root"].signed.version += 1
 
 roles["root"].signatures.clear()
 for key in [keys["root"], another_root_key, new_root_key]:
     roles["root"].sign(SSlibSigner(key), append=True)
```

### Comparing `tuf-2.1.0/examples/manual_repo/hashed_bin_delegation.py` & `tuf-3.0.0/examples/manual_repo/hashed_bin_delegation.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,19 @@
 import os
 import tempfile
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Tuple
 
 from securesystemslib.keys import generate_ed25519_key
-from securesystemslib.signer import SSlibSigner
+from securesystemslib.signer import SSlibKey, SSlibSigner
 
 from tuf.api.metadata import (
     DelegatedRole,
     Delegations,
-    Key,
     Metadata,
     TargetFile,
     Targets,
 )
 from tuf.api.serialization.json import JSONSerializer
 
 
@@ -75,14 +74,15 @@
 NUMBER_OF_PREFIXES = 16**PREFIX_LEN  # ... 256 prefixes, i.e. 00, 01, ..., ff.
 #
 # If the number of bins is a power of two, hash prefixes are evenly distributed
 # over all bins, which allows to calculate the uniform size of ...
 BIN_SIZE = NUMBER_OF_PREFIXES // NUMBER_OF_BINS  # ... 8, where each bin is
 # responsible for a range of 8 prefixes, i.e. 00-07, 08-0f, ..., f8-ff.
 
+
 # Helpers
 # -------
 def _bin_name(low: int, high: int) -> str:
     """Generates a bin name according to the hash prefixes the bin serves.
 
     The name is either a single hash prefix for bin size 1, or a range of hash
     prefixes otherwise. The prefix length is needed to zero-left-pad the
@@ -142,15 +142,15 @@
 # -------------
 # NOTE: See "Targets" and "Targets delegation" paragraphs in 'basic_repo.py'
 # example for more details about the Targets object.
 
 # Create preliminary delegating targets role (bins) and add public key for
 # delegated targets (bin_n) to key store. Delegation details are update below.
 roles["bins"] = Metadata(Targets(expires=_in(365)))
-bin_n_key = Key.from_securesystemslib_key(keys["bin-n"])
+bin_n_key = SSlibKey.from_securesystemslib_key(keys["bin-n"])
 roles["bins"].signed.delegations = Delegations(
     keys={bin_n_key.keyid: bin_n_key},
     roles={},
 )
 
 # The hash bin generator yields an ordered list of incremental hash bin names
 # (ranges), plus the hash prefixes each bin is responsible for, e.g.:
```

### Comparing `tuf-2.1.0/examples/manual_repo/succinct_hash_bin_delegations.py` & `tuf-3.0.0/examples/manual_repo/succinct_hash_bin_delegations.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import tempfile
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Dict, Tuple
 
 from securesystemslib.keys import generate_ed25519_key
-from securesystemslib.signer import SSlibSigner
+from securesystemslib.signer import SSlibKey, SSlibSigner
 
 from tuf.api.metadata import (
     Delegations,
     Key,
     Metadata,
     SuccinctRoles,
     TargetFile,
@@ -78,15 +78,15 @@
 # network overhead. For the purpose of this example only one key is required.
 THRESHOLD = 1
 
 
 def create_key() -> Tuple[Key, SSlibSigner]:
     """Generates a new Key and Signer."""
     sslib_key = generate_ed25519_key()
-    return Key.from_securesystemslib_key(sslib_key), SSlibSigner(sslib_key)
+    return SSlibKey.from_securesystemslib_key(sslib_key), SSlibSigner(sslib_key)
 
 
 # Create one signing key for all bins, and one for the delegating targets role.
 bins_key, bins_signer = create_key()
 _, targets_signer = create_key()
 
 # Delegating targets role
```

### Comparing `tuf-2.1.0/examples/repository/_simplerepo.py` & `tuf-3.0.0/examples/repository/repo`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,142 @@
+#!/usr/bin/env python
 # Copyright 2021-2022 python-tuf contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
-"""Simple example of using the repository library to build a repository"""
+"""Simple repository example application
 
-import copy
+The application stores metadata and targets in memory, and serves them via http.
+Nothing is persisted on disk or loaded from disk. The application simulates a
+live repository by adding new target files periodically.
+"""
+
+import argparse
 import logging
-from collections import defaultdict
-from datetime import datetime, timedelta
+import sys
+from datetime import datetime
+from http.server import BaseHTTPRequestHandler, ThreadingHTTPServer
+from time import time
 from typing import Dict, List
 
-from securesystemslib import keys
-from securesystemslib.signer import Signer, SSlibSigner
+from _simplerepo import SimpleRepository
 
-from tuf.api.metadata import (
-    Key,
-    Metadata,
-    MetaFile,
-    Root,
-    Snapshot,
-    TargetFile,
-    Targets,
-    Timestamp,
-)
-from tuf.repository import Repository
+from tuf.api.serialization.json import JSONSerializer
 
 logger = logging.getLogger(__name__)
 
-_signed_init = {
-    Root.type: Root,
-    Snapshot.type: Snapshot,
-    Targets.type: Targets,
-    Timestamp.type: Timestamp,
-}
-
-
-class SimpleRepository(Repository):
-    """Very simple in-memory repository implementation
-
-    This repository keeps the metadata for all versions of all roles in memory.
-    It also keeps all target content in memory.
-
-
-    Attributes:
-        role_cache: Every historical metadata version of every role in this
-            repository. Keys are role names and values are lists of Metadata
-        signer_cache: All signers available to the repository. Keys are role
-            names, values are lists of signers
-        target_cache: All target files served by the repository. Keys are
-            target paths and values are file contents as bytes.
+
+class ReqHandler(BaseHTTPRequestHandler):
+    """HTTP handler for the repository example application
+
+    Serves metadata, targets and a small upload API using a SimpleRepository
     """
 
-    expiry_period = timedelta(days=1)
+    def do_POST(self):
+        """Handle POST requests, aka the 'uploader API'"""
+
+        content_len = int(self.headers.get("content-length", 0))
+        data = self.rfile.read(content_len)
+
+        if self.path.startswith("/api/delegation/"):
+            role = self.path[len("/api/delegation/") :]
+            if not self.server.repo.submit_delegation(role, data):
+                return self.send_error(400, f"Failed to delegate to {role}")
+        elif self.path.startswith("/api/role/"):
+            role = self.path[len("/api/role/") :]
+            if not self.server.repo.submit_role(role, data):
+                return self.send_error(400, f"Failed to submit role {role}")
+        else:
+            return self.send_error(404)
+
+        self.send_response(200)
+        self.end_headers()
+
+    def do_GET(self):
+        """Handle GET: metadata and target files"""
+        data = None
+
+        if self.path.startswith("/metadata/") and self.path.endswith(".json"):
+            data = self.get_metadata(
+                self.path[len("/metadata/") : -len(".json")]
+            )
+        elif self.path.startswith("/targets/"):
+            data = self.get_target(self.path[len("/targets/") :])
+
+        if data is None:
+            self.send_error(404)
+        else:
+            self.send_response(200)
+            self.send_header("Content-length", len(data))
+            self.end_headers()
+            self.wfile.write(data)
+
+    def get_metadata(self, ver_and_role: str):
+        repo = self.server.repo
+
+        ver_str, sep, role = ver_and_role.rpartition(".")
+        if sep == "":
+            # 0 will lead to list lookup with -1, meaning latest version
+            ver = 0
+        else:
+            ver = int(ver_str)
+
+        if role not in repo.role_cache or ver > len(repo.role_cache[role]):
+            return None
+
+        # return metadata
+        return repo.role_cache[role][ver - 1].to_bytes(JSONSerializer())
+
+    def get_target(self, targetpath: str):
+        repo = self.server.repo
+
+        # unimplement the dumb hashing scheme
+        # TODO: maybe use hashed paths as the target_cache key
+        dir, sep, hashname = targetpath.rpartition("/")
+        _, _, name = hashname.partition(".")
+        target = f"{dir}{sep}{name}"
+
+        if target not in repo.target_cache:
+            return None
+
+        # send the target content
+        return repo.target_cache[target]
+
+
+class RepositoryServer(ThreadingHTTPServer):
+    def __init__(self, port: int):
+        super().__init__(("127.0.0.1", port), ReqHandler)
+        self.timeout = 1
+        self.repo = SimpleRepository()
+
+
+def main(argv: List[str]) -> None:
+    """Example repository server"""
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-v", "--verbose", action="count")
+    parser.add_argument("-p", "--port", type=int, default=8001)
+    args, _ = parser.parse_known_args(argv)
+
+    level = logging.DEBUG if args.verbose else logging.INFO
+    logging.basicConfig(level=level)
+
+    server = RepositoryServer(args.port)
+    last_change = 0
+    counter = 0
+
+    logger.info(
+        f"Now serving. Root v1 at http://127.0.0.1:{server.server_port}/metadata/1.root.json"
+    )
+
+    while True:
+        # Simulate a live repository: Add a new target file every few seconds
+        if time() - last_change > 10:
+            last_change = int(time())
+            counter += 1
+            content = str(datetime.fromtimestamp(last_change))
+            server.repo.add_target(f"file{str(counter)}.txt", content)
+
+        server.handle_request()
+
 
-    def __init__(self) -> None:
-        # all versions of all metadata
-        self.role_cache: Dict[str, List[Metadata]] = defaultdict(list)
-        # all current keys
-        self.signer_cache: Dict[str, List[Signer]] = defaultdict(list)
-        # all target content
-        self.target_cache: Dict[str, bytes] = {}
-        # version cache for snapshot and all targets, updated in close().
-        # The 'defaultdict(lambda: ...)' trick allows close() to easily modify
-        # the version without always creating a new MetaFile
-        self._snapshot_info = MetaFile(1)
-        self._targets_infos: Dict[str, MetaFile] = defaultdict(
-            lambda: MetaFile(1)
-        )
-
-        # setup a basic repository, generate signing key per top-level role
-        with self.edit("root") as root:
-            for role in ["root", "timestamp", "snapshot", "targets"]:
-                key = keys.generate_ed25519_key()
-                self.signer_cache[role].append(SSlibSigner(key))
-                root.add_key(Key.from_securesystemslib_key(key), role)
-
-        for role in ["timestamp", "snapshot", "targets"]:
-            with self.edit(role):
-                pass
-
-    @property
-    def targets_infos(self) -> Dict[str, MetaFile]:
-        return self._targets_infos
-
-    @property
-    def snapshot_info(self) -> MetaFile:
-        return self._snapshot_info
-
-    def open(self, role: str) -> Metadata:
-        """Return current Metadata for role from 'storage' (or create a new one)"""
-
-        if role not in self.role_cache:
-            signed_init = _signed_init.get(role, Targets)
-            md = Metadata(signed_init())
-
-            # this makes version bumping in close() simpler
-            md.signed.version = 0
-            return md
-
-        # return latest metadata from storage (but don't return a reference)
-        return copy.deepcopy(self.role_cache[role][-1])
-
-    def close(self, role: str, md: Metadata) -> None:
-        """Store a version of metadata. Handle version bumps, expiry, signing"""
-        md.signed.version += 1
-        md.signed.expires = datetime.utcnow() + self.expiry_period
-
-        md.signatures.clear()
-        for signer in self.signer_cache[role]:
-            md.sign(signer, append=True)
-
-        # store new metadata version, update version caches
-        self.role_cache[role].append(md)
-        if role == "snapshot":
-            self._snapshot_info.version = md.signed.version
-        elif role not in ["root", "timestamp"]:
-            self._targets_infos[f"{role}.json"].version = md.signed.version
-
-    def add_target(self, path: str, content: str) -> None:
-        """Add a target to repository"""
-        data = bytes(content, "utf-8")
-
-        # add content to cache for serving to clients
-        self.target_cache[path] = data
-
-        # add a target in the targets metadata
-        with self.edit("targets") as targets:
-            targets.targets[path] = TargetFile.from_data(path, data)
-
-        logger.debug("Targets v%d", targets.version)
-
-        # update snapshot, timestamp
-        self.snapshot()
-        self.timestamp()
+if __name__ == "__main__":
+    main(sys.argv)
```

### Comparing `tuf-2.1.0/tests/aggregate_tests.py` & `tuf-3.0.0/tests/aggregate_tests.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_simulator.py` & `tuf-3.0.0/tests/repository_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 import tempfile
 from dataclasses import dataclass, field
 from typing import Dict, Iterator, List, Optional, Tuple
 from urllib import parse
 
 import securesystemslib.hash as sslib_hash
 from securesystemslib.keys import generate_ed25519_key
-from securesystemslib.signer import SSlibSigner
+from securesystemslib.signer import SSlibKey, SSlibSigner
 
 from tuf.api.exceptions import DownloadHTTPError
 from tuf.api.metadata import (
     SPECIFICATION_VERSION,
     TOP_LEVEL_ROLE_NAMES,
     DelegatedRole,
     Delegations,
@@ -152,16 +152,16 @@
         """Yield role name and signed portion of targets one by one."""
         yield Targets.type, self.md_targets.signed
         for role, md in self.md_delegates.items():
             yield role, md.signed
 
     @staticmethod
     def create_key() -> Tuple[Key, SSlibSigner]:
-        sslib_key = generate_ed25519_key()
-        return Key.from_securesystemslib_key(sslib_key), SSlibSigner(sslib_key)
+        key = generate_ed25519_key()
+        return SSlibKey.from_securesystemslib_key(key), SSlibSigner(key)
 
     def add_signer(self, role: str, signer: SSlibSigner) -> None:
         if role not in self.signers:
             self.signers[role] = {}
         self.signers[role][signer.key_dict["keyid"]] = signer
 
     def rotate_keys(self, role: str) -> None:
```

### Comparing `tuf-2.1.0/tests/simple_server.py` & `tuf-3.0.0/tests/simple_server.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/test_api.py` & `tuf-3.0.0/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,31 +13,33 @@
 import sys
 import tempfile
 import unittest
 from copy import copy
 from datetime import datetime, timedelta
 from typing import Any, ClassVar, Dict
 
+from securesystemslib import exceptions as sslib_exceptions
 from securesystemslib import hash as sslib_hash
 from securesystemslib.interface import (
     import_ed25519_privatekey_from_file,
     import_ed25519_publickey_from_file,
 )
 from securesystemslib.keys import generate_ed25519_key
-from securesystemslib.signer import Signature, SSlibSigner
+from securesystemslib.signer import SSlibKey, SSlibSigner
 
 from tests import utils
 from tuf.api import exceptions
 from tuf.api.metadata import (
     TOP_LEVEL_ROLE_NAMES,
     DelegatedRole,
     Delegations,
     Key,
     Metadata,
     Root,
+    Signature,
     Snapshot,
     SuccinctRoles,
     TargetFile,
     Targets,
     Timestamp,
 )
 from tuf.api.serialization import DeserializationError, SerializationError
@@ -94,15 +96,14 @@
     def test_generic_read(self) -> None:
         for metadata, inner_metadata_cls in [
             (Root.type, Root),
             (Snapshot.type, Snapshot),
             (Timestamp.type, Timestamp),
             (Targets.type, Targets),
         ]:
-
             # Load JSON-formatted metdata of each supported type from file
             # and from out-of-band read JSON string
             path = os.path.join(self.repo_dir, "metadata", metadata + ".json")
             md_obj = Metadata.from_file(path)
             with open(path, "rb") as f:
                 md_obj2 = Metadata.from_bytes(f.read())
 
@@ -183,116 +184,112 @@
 
             # Case 2: test compact by using the default serializer.
             obj_bytes = md_obj.to_bytes()
             metadata_obj_2 = Metadata.from_bytes(obj_bytes)
             self.assertEqual(metadata_obj_2.to_bytes(), obj_bytes)
 
     def test_sign_verify(self) -> None:
-        root_path = os.path.join(self.repo_dir, "metadata", "root.json")
-        root = Metadata[Root].from_file(root_path).signed
+        path = os.path.join(self.repo_dir, "metadata")
+        root = Metadata[Root].from_file(os.path.join(path, "root.json")).signed
 
         # Locate the public keys we need from root
         targets_keyid = next(iter(root.roles[Targets.type].keyids))
         targets_key = root.keys[targets_keyid]
         snapshot_keyid = next(iter(root.roles[Snapshot.type].keyids))
         snapshot_key = root.keys[snapshot_keyid]
         timestamp_keyid = next(iter(root.roles[Timestamp.type].keyids))
         timestamp_key = root.keys[timestamp_keyid]
 
         # Load sample metadata (targets) and assert ...
-        path = os.path.join(self.repo_dir, "metadata", "targets.json")
-        md_obj = Metadata.from_file(path)
+        md_obj = Metadata.from_file(os.path.join(path, "targets.json"))
+        sig = md_obj.signatures[targets_keyid]
+        data = CanonicalJSONSerializer().serialize(md_obj.signed)
 
         # ... it has a single existing signature,
         self.assertEqual(len(md_obj.signatures), 1)
         # ... which is valid for the correct key.
-        targets_key.verify_signature(md_obj)
-        with self.assertRaises(exceptions.UnsignedMetadataError):
-            snapshot_key.verify_signature(md_obj)
-
-        # Test verifying with explicitly set serializer
-        targets_key.verify_signature(md_obj, CanonicalJSONSerializer())
-        with self.assertRaises(exceptions.UnsignedMetadataError):
-            targets_key.verify_signature(md_obj, JSONSerializer())  # type: ignore[arg-type]
+        targets_key.verify_signature(sig, data)
+        with self.assertRaises(sslib_exceptions.VerificationError):
+            snapshot_key.verify_signature(sig, data)
 
         sslib_signer = SSlibSigner(self.keystore[Snapshot.type])
         # Append a new signature with the unrelated key and assert that ...
-        sig = md_obj.sign(sslib_signer, append=True)
+        snapshot_sig = md_obj.sign(sslib_signer, append=True)
         # ... there are now two signatures, and
         self.assertEqual(len(md_obj.signatures), 2)
         # ... both are valid for the corresponding keys.
-        targets_key.verify_signature(md_obj)
-        snapshot_key.verify_signature(md_obj)
+        targets_key.verify_signature(sig, data)
+        snapshot_key.verify_signature(snapshot_sig, data)
         # ... the returned (appended) signature is for snapshot key
-        self.assertEqual(sig.keyid, snapshot_keyid)
+        self.assertEqual(snapshot_sig.keyid, snapshot_keyid)
 
         sslib_signer = SSlibSigner(self.keystore[Timestamp.type])
         # Create and assign (don't append) a new signature and assert that ...
-        md_obj.sign(sslib_signer, append=False)
+        ts_sig = md_obj.sign(sslib_signer, append=False)
         # ... there now is only one signature,
         self.assertEqual(len(md_obj.signatures), 1)
         # ... valid for that key.
-        timestamp_key.verify_signature(md_obj)
-        with self.assertRaises(exceptions.UnsignedMetadataError):
-            targets_key.verify_signature(md_obj)
+        timestamp_key.verify_signature(ts_sig, data)
+        with self.assertRaises(sslib_exceptions.VerificationError):
+            targets_key.verify_signature(ts_sig, data)
 
     def test_sign_failures(self) -> None:
         # Test throwing UnsignedMetadataError because of signing problems
         # related to bad information in the signer.
         md = Metadata.from_file(
             os.path.join(self.repo_dir, "metadata", "snapshot.json")
         )
         key_dict = copy(self.keystore[Snapshot.type])
         key_dict["keytype"] = "rsa"
         key_dict["scheme"] = "bad_scheme"
         sslib_signer = SSlibSigner(key_dict)
         with self.assertRaises(exceptions.UnsignedMetadataError):
             md.sign(sslib_signer)
 
-    def test_verify_failures(self) -> None:
+    def test_key_verify_failures(self) -> None:
         root_path = os.path.join(self.repo_dir, "metadata", "root.json")
         root = Metadata[Root].from_file(root_path).signed
 
         # Locate the timestamp public key we need from root
         timestamp_keyid = next(iter(root.roles[Timestamp.type].keyids))
         timestamp_key = root.keys[timestamp_keyid]
 
         # Load sample metadata (timestamp)
         path = os.path.join(self.repo_dir, "metadata", "timestamp.json")
         md_obj = Metadata.from_file(path)
+        sig = md_obj.signatures[timestamp_keyid]
+        data = CanonicalJSONSerializer().serialize(md_obj.signed)
 
         # Test failure on unknown scheme (securesystemslib
         # UnsupportedAlgorithmError)
         scheme = timestamp_key.scheme
         timestamp_key.scheme = "foo"
-        with self.assertRaises(exceptions.UnsignedMetadataError):
-            timestamp_key.verify_signature(md_obj)
+        with self.assertRaises(sslib_exceptions.VerificationError):
+            timestamp_key.verify_signature(sig, data)
         timestamp_key.scheme = scheme
 
         # Test failure on broken public key data (securesystemslib
         # CryptoError)
         public = timestamp_key.keyval["public"]
         timestamp_key.keyval["public"] = "ffff"
-        with self.assertRaises(exceptions.UnsignedMetadataError):
-            timestamp_key.verify_signature(md_obj)
+        with self.assertRaises(sslib_exceptions.VerificationError):
+            timestamp_key.verify_signature(sig, data)
         timestamp_key.keyval["public"] = public
 
         # Test failure with invalid signature (securesystemslib
         # FormatError)
-        sig = md_obj.signatures[timestamp_keyid]
-        correct_sig = sig.signature
-        sig.signature = "foo"
-        with self.assertRaises(exceptions.UnsignedMetadataError):
-            timestamp_key.verify_signature(md_obj)
+        incorrect_sig = copy(sig)
+        incorrect_sig.signature = "foo"
+        with self.assertRaises(sslib_exceptions.VerificationError):
+            timestamp_key.verify_signature(incorrect_sig, data)
 
         # Test failure with valid but incorrect signature
-        sig.signature = "ff" * 64
-        with self.assertRaises(exceptions.UnsignedMetadataError):
-            timestamp_key.verify_signature(md_obj)
-        sig.signature = correct_sig
+        incorrect_sig.signature = "ff" * 64
+        with self.assertRaises(sslib_exceptions.UnverifiedSignatureError):
+            timestamp_key.verify_signature(incorrect_sig, data)
 
     def test_metadata_signed_is_expired(self) -> None:
         # Use of Snapshot is arbitrary, we're just testing the base class
         # features with real data
         snapshot_path = os.path.join(self.repo_dir, "metadata", "snapshot.json")
         md = Metadata.from_file(snapshot_path)
 
@@ -351,14 +348,23 @@
         # verify fails when delegate content is modified
         expires = snapshot.signed.expires
         snapshot.signed.expires = expires + timedelta(days=1)
         with self.assertRaises(exceptions.UnsignedMetadataError):
             root.verify_delegate(Snapshot.type, snapshot)
         snapshot.signed.expires = expires
 
+        # verify fails if sslib verify fails with VerificationError
+        # (in this case signature is malformed)
+        keyid = next(iter(root.signed.roles[Snapshot.type].keyids))
+        good_sig = snapshot.signatures[keyid].signature
+        snapshot.signatures[keyid].signature = "foo"
+        with self.assertRaises(exceptions.UnsignedMetadataError):
+            root.verify_delegate(Snapshot.type, snapshot)
+        snapshot.signatures[keyid].signature = good_sig
+
         # verify fails if roles keys do not sign the metadata
         with self.assertRaises(exceptions.UnsignedMetadataError):
             root.verify_delegate(Timestamp.type, snapshot)
 
         # Add a key to snapshot role, make sure the new sig fails to verify
         ts_keyid = next(iter(root.signed.roles[Timestamp.type].keyids))
         root.signed.add_key(root.signed.keys[ts_keyid], Snapshot.type)
@@ -378,45 +384,40 @@
         snapshot.sign(SSlibSigner(self.keystore[Timestamp.type]), append=True)
         root.verify_delegate(Snapshot.type, snapshot)
 
     def test_key_class(self) -> None:
         # Test if from_securesystemslib_key removes the private key from keyval
         # of a securesystemslib key dictionary.
         sslib_key = generate_ed25519_key()
-        key = Key.from_securesystemslib_key(sslib_key)
+        key = SSlibKey.from_securesystemslib_key(sslib_key)
         self.assertFalse("private" in key.keyval.keys())
 
-        # Test raising ValueError with non-existent keytype
-        sslib_key["keytype"] = "bad keytype"
-        with self.assertRaises(ValueError):
-            Key.from_securesystemslib_key(sslib_key)
-
     def test_root_add_key_and_revoke_key(self) -> None:
         root_path = os.path.join(self.repo_dir, "metadata", "root.json")
         root = Metadata[Root].from_file(root_path)
 
         # Create a new key
         root_key2 = import_ed25519_publickey_from_file(
             os.path.join(self.keystore_dir, "root_key2.pub")
         )
         keyid = root_key2["keyid"]
-        key_metadata = Key(
+        key_metadata = SSlibKey(
             keyid,
             root_key2["keytype"],
             root_key2["scheme"],
             root_key2["keyval"],
         )
 
         # Assert that root does not contain the new key
         self.assertNotIn(keyid, root.signed.roles[Root.type].keyids)
         self.assertNotIn(keyid, root.signed.keys)
 
         # Assert that add_key with old argument order will raise an error
         with self.assertRaises(ValueError):
-            root.signed.add_key(Root.type, key_metadata)  # type: ignore
+            root.signed.add_key(Root.type, key_metadata)
 
         # Add new root key
         root.signed.add_key(key_metadata, Root.type)
 
         # Assert that key is added
         self.assertIn(keyid, root.signed.roles[Root.type].keyids)
         self.assertIn(keyid, root.signed.keys)
@@ -509,15 +510,15 @@
             },
             "scheme": "ed25519",
         }
         key = Key.from_dict("id2", key_dict)
 
         # Assert that add_key with old argument order will raise an error
         with self.assertRaises(ValueError):
-            targets.add_key("role1", key)  # type: ignore
+            targets.add_key("role1", key)
 
         # Assert that delegated role "role1" does not contain the new key
         self.assertNotIn(key.keyid, targets.delegations.roles["role1"].keyids)
         targets.add_key(key, "role1")
 
         # Assert that the new key is added to the delegated role "role1"
         self.assertIn(key.keyid, targets.delegations.roles["role1"].keyids)
@@ -607,15 +608,14 @@
         self.assertEqual(len(targets.delegations.keys), 0)
 
         # Try removing it again.
         with self.assertRaises(ValueError):
             targets.revoke_key(key.keyid)
 
     def test_length_and_hash_validation(self) -> None:
-
         # Test metadata files' hash and length verification.
         # Use timestamp to get a MetaFile object and snapshot
         # for untrusted metadata file to verify.
         timestamp_path = os.path.join(
             self.repo_dir, "metadata", "timestamp.json"
         )
         timestamp = Metadata[Timestamp].from_file(timestamp_path)
@@ -721,14 +721,42 @@
         )
         targetfile_from_data.verify_length_and_hashes(data)
 
         # Test with no algorithms specified
         targetfile_from_data = TargetFile.from_data(target_file_path, data)
         targetfile_from_data.verify_length_and_hashes(data)
 
+    def test_targetfile_get_prefixed_paths(self) -> None:
+        target = TargetFile(100, {"sha256": "abc", "md5": "def"}, "a/b/f.ext")
+        self.assertEqual(
+            target.get_prefixed_paths(), ["a/b/abc.f.ext", "a/b/def.f.ext"]
+        )
+
+        target = TargetFile(100, {"sha256": "abc", "md5": "def"}, "")
+        self.assertEqual(target.get_prefixed_paths(), ["abc.", "def."])
+
+        target = TargetFile(100, {"sha256": "abc", "md5": "def"}, "a/b/")
+        self.assertEqual(target.get_prefixed_paths(), ["a/b/abc.", "a/b/def."])
+
+        target = TargetFile(100, {"sha256": "abc", "md5": "def"}, "f.ext")
+        self.assertEqual(
+            target.get_prefixed_paths(), ["abc.f.ext", "def.f.ext"]
+        )
+
+        target = TargetFile(100, {"sha256": "abc", "md5": "def"}, "a/b/.ext")
+        self.assertEqual(
+            target.get_prefixed_paths(), ["a/b/abc..ext", "a/b/def..ext"]
+        )
+
+        target = TargetFile(100, {"sha256": "abc"}, "/root/file.ext")
+        self.assertEqual(target.get_prefixed_paths(), ["/root/abc.file.ext"])
+
+        target = TargetFile(100, {"sha256": "abc"}, "/")
+        self.assertEqual(target.get_prefixed_paths(), ["/abc."])
+
     def test_is_delegated_role(self) -> None:
         # test path matches
         # see more extensive tests in test_is_target_in_pathpattern()
         for paths in [
             ["a/path"],
             ["otherpath", "a/path"],
             ["*/?ath"],
```

### Comparing `tuf-2.1.0/tests/test_examples.py` & `tuf-3.0.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/test_fetcher_ng.py` & `tuf-3.0.0/tests/test_fetcher_ng.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/test_metadata_eq_.py` & `tuf-3.0.0/tests/test_metadata_eq_.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 import copy
 import os
 import sys
 import unittest
 from typing import Any, ClassVar, Dict
 
-from securesystemslib.signer import Signature
+from securesystemslib.signer import SSlibKey
 
 from tests import utils
 from tuf.api.metadata import (
     TOP_LEVEL_ROLE_NAMES,
     DelegatedRole,
     Delegations,
-    Key,
     Metadata,
     MetaFile,
     Role,
+    Signature,
     SuccinctRoles,
     TargetFile,
 )
 
 
 class TestMetadataComparisions(unittest.TestCase):
     """Test __eq__ for all classes inside tuf/api/metadata.py."""
@@ -46,15 +46,15 @@
         for md in TOP_LEVEL_ROLE_NAMES:
             with open(os.path.join(cls.repo_dir, f"{md}.json"), "rb") as f:
                 data = f.read()
                 cls.objects[md.capitalize()] = Metadata.from_bytes(data).signed
 
         cls.objects["Metadata"] = Metadata(cls.objects["Timestamp"], {})
         cls.objects["Signed"] = cls.objects["Timestamp"]
-        cls.objects["Key"] = Key(
+        cls.objects["Key"] = SSlibKey(
             "id", "rsa", "rsassa-pss-sha256", {"public": "foo"}
         )
         cls.objects["Role"] = Role(["keyid1", "keyid2"], 3)
         cls.objects["MetaFile"] = MetaFile(1, 12, {"sha256": "abc"})
         cls.objects["DelegatedRole"] = DelegatedRole("a", [], 1, False, ["d"])
         cls.objects["SuccinctRoles"] = SuccinctRoles(["keyid"], 1, 8, "foo")
         cls.objects["Delegations"] = Delegations(
```

### Comparing `tuf-2.1.0/tests/test_metadata_generation.py` & `tuf-3.0.0/tests/test_metadata_generation.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/test_metadata_serialization.py` & `tuf-3.0.0/tests/test_metadata_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         "scheme wrong type": '{"keyid": "id", "keytype": "rsa", "scheme": 1, "keyval": {"public": "abc"}}',
         "keyval wrong type": '{"keyid": "id", "keytype": "rsa", "scheme": "rsassa-pss-sha256", "keyval": 1}',
     }
 
     @utils.run_sub_tests_with_dataset(invalid_keys)
     def test_invalid_key_serialization(self, test_case_data: str) -> None:
         case_dict = json.loads(test_case_data)
-        with self.assertRaises((TypeError, KeyError)):
+        with self.assertRaises((TypeError, KeyError, ValueError)):
             keyid = case_dict.pop("keyid")
             Key.from_dict(keyid, case_dict)
 
     invalid_roles: utils.DataSet = {
         "no threshold": '{"keyids": ["keyid"]}',
         "no keyids": '{"threshold": 3}',
         "wrong threshold type": '{"keyids": ["keyid"], "threshold": "a"}',
```

### Comparing `tuf-2.1.0/tests/test_trusted_metadata_set.py` & `tuf-3.0.0/tests/test_trusted_metadata_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     Timestamp,
 )
 from tuf.api.serialization.json import JSONSerializer
 from tuf.ngclient._internal.trusted_metadata_set import TrustedMetadataSet
 
 logger = logging.getLogger(__name__)
 
+
 # pylint: disable=too-many-public-methods
 class TestTrustedMetadataSet(unittest.TestCase):
     """Tests for all public API of the TrustedMetadataSet class."""
 
     keystore: ClassVar[Dict[str, SSlibSigner]]
     metadata: ClassVar[Dict[str, bytes]]
     repo_dir: ClassVar[str]
@@ -455,14 +456,15 @@
         )
         # new_delegate.signed.version != meta.version stored in snapshot
         with self.assertRaises(exceptions.BadVersionNumberError):
             self.trusted_set.update_targets(self.metadata[Targets.type])
 
     def test_update_targets_expired_new_target(self) -> None:
         self._update_all_besides_targets()
+
         # new_delegated_target has expired
         def target_expired_modifier(target: Targets) -> None:
             target.expires = datetime(1970, 1, 1)
 
         targets = self.modify_metadata(Targets.type, target_expired_modifier)
         with self.assertRaises(exceptions.ExpiredMetadataError):
             self.trusted_set.update_targets(targets)
```

### Comparing `tuf-2.1.0/tests/test_updater_consistent_snapshot.py` & `tuf-3.0.0/tests/test_updater_consistent_snapshot.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/test_updater_delegation_graphs.py` & `tuf-3.0.0/tests/test_updater_delegation_graphs.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/test_updater_fetch_target.py` & `tuf-3.0.0/tests/test_updater_fetch_target.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/test_updater_key_rotations.py` & `tuf-3.0.0/tests/test_updater_key_rotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,14 @@
         Assert that refresh() result is expected and that local metadata on disk
         is the expected one after all roots have been loaded from remote using
         the standard client update workflow.
         """
         self.setup_subtest()
         roles = ["timestamp", "snapshot", "targets"]
         for role in roles:
-
             # clear role keys, signers
             self.sim.root.roles[role].keyids.clear()
             self.sim.signers[role].clear()
 
             self.sim.root.roles[role].threshold = md_version.threshold
             for i in md_version.keys:
                 self.sim.root.add_key(self.keys[i], role)
```

### Comparing `tuf-2.1.0/tests/test_updater_ng.py` & `tuf-3.0.0/tests/test_updater_ng.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/test_updater_top_level_update.py` & `tuf-3.0.0/tests/test_updater_top_level_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,14 @@
         # Should fail as a new version of snapshot will be fetched which lowers
         # the snapshot.meta["targets.json"] version by 1 and throws an error.
         with self.assertRaises(BadVersionNumberError):
             self._run_refresh()
 
     @patch.object(builtins, "open", wraps=builtins.open)
     def test_load_metadata_from_cache(self, wrapped_open: MagicMock) -> None:
-
         # Add new delegated targets
         spec_version = ".".join(SPECIFICATION_VERSION)
         targets = Targets(1, spec_version, self.sim.safe_expiry, {}, None)
         role = DelegatedRole("role1", [], 1, False, ["*"], None)
         self.sim.add_delegation("targets", role, targets)
         self.sim.update_snapshot()
```

### Comparing `tuf-2.1.0/tests/test_updater_validation.py` & `tuf-3.0.0/tests/test_updater_validation.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/test_utils.py` & `tuf-3.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/utils.py` & `tuf-3.0.0/tests/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
 # Used when forming URLs on the client side
 TEST_HOST_ADDRESS = "127.0.0.1"
 
 # DataSet is only here so type hints can be used.
 DataSet = Dict[str, Any]
 
+
 # Test runner decorator: Runs the test as a set of N SubTests,
 # (where N is number of items in dataset), feeding the actual test
 # function one test case at a time
 def run_sub_tests_with_dataset(
     dataset: DataSet,
 ) -> Callable[[Callable], Callable]:
     """Decorator starting a unittest.TestCase.subtest() for each of the
@@ -183,15 +184,14 @@
         self,
         log: logging.Logger,
         server: str = os.path.join(TESTS_DIR, "simple_server.py"),
         timeout: int = 10,
         popen_cwd: str = ".",
         extra_cmd_args: Optional[List[str]] = None,
     ):
-
         self.server = server
         self.__logger = log
         # Stores popped messages from the queue.
         self.__logged_messages: List[str] = []
         self.__server_process: Optional[subprocess.Popen] = None
         self._log_queue: Optional[queue.Queue] = None
         self.port = -1
```

### Comparing `tuf-2.1.0/tests/generated_data/generate_md.py` & `tuf-3.0.0/tests/generated_data/generate_md.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 import os
 import sys
 from datetime import datetime
 from typing import Dict, List, Optional
 
-from securesystemslib.signer import SSlibSigner
+from securesystemslib.signer import SSlibKey, SSlibSigner
 
 from tests import utils
 from tuf.api.metadata import Key, Metadata, Root, Snapshot, Targets, Timestamp
 from tuf.api.serialization.json import JSONSerializer
 
 # Hardcode keys and expiry time to achieve reproducibility.
 public_values: List[str] = [
@@ -32,15 +32,15 @@
     "09d440e3725cec247dcb8703b646a87dd2a4d75343e8095c036c32795eefe3b9",
     "3458204ed467519c19a5316eb278b5608472a1bbf15850ebfb462d5315e4f86d",
     "2be5c21e3614f9f178fb49c4a34d0c18ffac30abd14ced917c60a52c8d8094b7",
 ]
 
 keys: Dict[str, Key] = {}
 for index in range(4):
-    keys[f"ed25519_{index}"] = Key.from_securesystemslib_key(
+    keys[f"ed25519_{index}"] = SSlibKey.from_securesystemslib_key(
         {
             "keytype": "ed25519",
             "scheme": "ed25519",
             "keyid": keyids[index],
             "keyval": {
                 "public": public_values[index],
                 "private": private_values[index],
```

### Comparing `tuf-2.1.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json` & `tuf-3.0.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/README.md` & `tuf-3.0.0/tests/repository_data/README.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/role1.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/root.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/targets.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/root.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json` & `tuf-3.0.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/role1.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/root.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/targets.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/root.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json` & `tuf-3.0.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/fishy_rolenames/metadata/1.root.json` & `tuf-3.0.0/tests/repository_data/fishy_rolenames/metadata/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json` & `tuf-3.0.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json` & `tuf-3.0.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/keystore/delegation_key` & `tuf-3.0.0/tests/repository_data/keystore/delegation_key`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/keystore/root_key` & `tuf-3.0.0/tests/repository_data/keystore/root_key`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/keystore/root_key.pub` & `tuf-3.0.0/tests/repository_data/keystore/root_key.pub`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/keystore/root_key2` & `tuf-3.0.0/tests/repository_data/keystore/root_key2`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/keystore/root_key3` & `tuf-3.0.0/tests/repository_data/keystore/root_key3`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/keystore/snapshot_key` & `tuf-3.0.0/tests/repository_data/keystore/snapshot_key`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/keystore/targets_key` & `tuf-3.0.0/tests/repository_data/keystore/targets_key`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/keystore/timestamp_key` & `tuf-3.0.0/tests/repository_data/keystore/timestamp_key`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/project/test-flat/project.cfg` & `tuf-3.0.0/tests/repository_data/project/test-flat/project.cfg`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/project/test-flat/test-flat.json` & `tuf-3.0.0/tests/repository_data/project/test-flat/test-flat.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata/1.root.json` & `tuf-3.0.0/tests/repository_data/repository/metadata/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata/role1.json` & `tuf-3.0.0/tests/repository_data/repository/metadata/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata/root.json` & `tuf-3.0.0/tests/repository_data/repository/metadata/root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata/snapshot.json` & `tuf-3.0.0/tests/repository_data/repository/metadata/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata/targets.json` & `tuf-3.0.0/tests/repository_data/repository/metadata/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata/timestamp.json` & `tuf-3.0.0/tests/repository_data/repository/metadata/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata.staged/1.root.json` & `tuf-3.0.0/tests/repository_data/repository/metadata.staged/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata.staged/role1.json` & `tuf-3.0.0/tests/repository_data/repository/metadata.staged/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata.staged/root.json` & `tuf-3.0.0/tests/repository_data/repository/metadata.staged/root.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata.staged/snapshot.json` & `tuf-3.0.0/tests/repository_data/repository/metadata.staged/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata.staged/targets.json` & `tuf-3.0.0/tests/repository_data/repository/metadata.staged/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tests/repository_data/repository/metadata.staged/timestamp.json` & `tuf-3.0.0/tests/repository_data/repository/metadata.staged/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tuf/api/exceptions.py` & `tuf-3.0.0/tuf/api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 
 # pylint: disable=unused-import
 from securesystemslib.exceptions import StorageError
 
 
 class RepositoryError(Exception):
     """An error with a repository's state, such as a missing file.
+
     It covers all exceptions that come from the repository side when
-    looking from the perspective of users of metadata API or ngclient."""
+    looking from the perspective of users of metadata API or ngclient.
+    """
 
 
 class UnsignedMetadataError(RepositoryError):
-    """An error about metadata object with insufficient threshold of
-    signatures."""
+    """An error about metadata object with insufficient threshold of signatures."""
 
 
 class BadVersionNumberError(RepositoryError):
     """An error for metadata that contains an invalid version number."""
 
 
 class EqualVersionNumberError(BadVersionNumberError):
```

### Comparing `tuf-2.1.0/tuf/api/metadata.py` & `tuf-3.0.0/tuf/api/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,24 +49,22 @@
     TypeVar,
     Union,
     cast,
 )
 
 from securesystemslib import exceptions as sslib_exceptions
 from securesystemslib import hash as sslib_hash
-from securesystemslib import keys as sslib_keys
-from securesystemslib.signer import Signature, Signer
+from securesystemslib.signer import Key, Signature, Signer
 from securesystemslib.storage import FilesystemBackend, StorageBackendInterface
 from securesystemslib.util import persist_temp_file
 
-from tuf.api import exceptions
+from tuf.api.exceptions import LengthOrHashMismatchError, UnsignedMetadataError
 from tuf.api.serialization import (
     MetadataDeserializer,
     MetadataSerializer,
-    SerializationError,
     SignedSerializer,
 )
 
 _ROOT = "root"
 _SNAPSHOT = "snapshot"
 _TARGETS = "targets"
 _TIMESTAMP = "timestamp"
@@ -216,15 +214,15 @@
             deserializer: ``MetadataDeserializer`` subclass instance that
                 implements the desired wireline format deserialization. Per
                 default a ``JSONDeserializer`` is used.
             storage_backend: Object that implements
                 ``securesystemslib.storage.StorageBackendInterface``.
                 Default is ``FilesystemBackend`` (i.e. a local file).
         Raises:
-            exceptions.StorageError: The file cannot be read.
+            StorageError: The file cannot be read.
             tuf.api.serialization.DeserializationError:
                 The file cannot be deserialized.
 
         Returns:
             TUF ``Metadata`` object.
         """
 
@@ -326,15 +324,15 @@
                 desired serialization format. Default is ``JSONSerializer``.
             storage_backend: ``StorageBackendInterface`` implementation. Default
                 is ``FilesystemBackend`` (i.e. a local file).
 
         Raises:
             tuf.api.serialization.SerializationError:
                 The metadata object cannot be serialized.
-            exceptions.StorageError: The file cannot be written.
+            StorageError: The file cannot be written.
         """
 
         bytes_data = self.to_bytes(serializer)
 
         with tempfile.TemporaryFile() as temp_file:
             temp_file.write(bytes_data)
             persist_temp_file(temp_file, filename, storage_backend)
@@ -357,15 +355,15 @@
                 default behavior is to replace signatures.
             signed_serializer: ``SignedSerializer`` that implements the desired
                 serialization format. Default is ``CanonicalJSONSerializer``.
 
         Raises:
             tuf.api.serialization.SerializationError:
                 ``signed`` cannot be serialized.
-            exceptions.UnsignedMetadataError: Signing errors.
+            UnsignedMetadataError: Signing errors.
 
         Returns:
             ``securesystemslib.signer.Signature`` object that was added into
             signatures.
         """
 
         if signed_serializer is None:
@@ -376,17 +374,15 @@
             signed_serializer = CanonicalJSONSerializer()
 
         bytes_data = signed_serializer.serialize(self.signed)
 
         try:
             signature = signer.sign(bytes_data)
         except Exception as e:
-            raise exceptions.UnsignedMetadataError(
-                "Problem signing the metadata"
-            ) from e
+            raise UnsignedMetadataError("Problem signing the metadata") from e
 
         if not append:
             self.signatures.clear()
 
         self.signatures[signature.keyid] = signature
 
         return signature
@@ -409,51 +405,48 @@
         Raises:
             UnsignedMetadataError: ``delegated_role`` was not signed with
                 required threshold of keys for ``role_name``.
             ValueError: no delegation was found for ``delegated_role``.
             TypeError: called this function on non-delegating metadata class.
         """
 
-        # Find the keys and role in delegator metadata
-        role: Optional[Role] = None
-        if isinstance(self.signed, Root):
-            keys = self.signed.keys
-            role = self.signed.roles.get(delegated_role)
-        elif isinstance(self.signed, Targets):
-            if self.signed.delegations is None:
-                raise ValueError(f"No delegation found for {delegated_role}")
-
-            keys = self.signed.delegations.keys
-            if self.signed.delegations.roles is not None:
-                role = self.signed.delegations.roles.get(delegated_role)
-            elif self.signed.delegations.succinct_roles is not None:
-                if self.signed.delegations.succinct_roles.is_delegated_role(
-                    delegated_role
-                ):
-                    role = self.signed.delegations.succinct_roles
-        else:
+        if self.signed.type not in ["root", "targets"]:
             raise TypeError("Call is valid only on delegator metadata")
 
-        if role is None:
-            raise ValueError(f"No delegation found for {delegated_role}")
+        if signed_serializer is None:
+            # pylint: disable=import-outside-toplevel
+            from tuf.api.serialization.json import CanonicalJSONSerializer
+
+            signed_serializer = CanonicalJSONSerializer()
+
+        data = signed_serializer.serialize(delegated_metadata.signed)
+        role = self.signed.get_delegated_role(delegated_role)
 
         # verify that delegated_metadata is signed by threshold of unique keys
         signing_keys = set()
         for keyid in role.keyids:
-            key = keys[keyid]
             try:
-                key.verify_signature(delegated_metadata, signed_serializer)
-                signing_keys.add(key.keyid)
-            except exceptions.UnsignedMetadataError:
-                logger.debug(
-                    "Key %s failed to verify %s", keyid, delegated_role
-                )
+                key = self.signed.get_key(keyid)
+            except ValueError:
+                logger.info("No key for keyid %s", keyid)
+                continue
+
+            if keyid not in delegated_metadata.signatures:
+                logger.info("No signature for keyid %s", keyid)
+                continue
+
+            sig = delegated_metadata.signatures[keyid]
+            try:
+                key.verify_signature(sig, data)
+                signing_keys.add(keyid)
+            except sslib_exceptions.UnverifiedSignatureError:
+                logger.info("Key %s failed to verify %s", keyid, delegated_role)
 
         if len(signing_keys) < role.threshold:
-            raise exceptions.UnsignedMetadataError(
+            raise UnsignedMetadataError(
                 f"{delegated_role} was signed by {len(signing_keys)}/"
                 f"{role.threshold} keys",
             )
 
 
 class Signed(metaclass=abc.ABCMeta):
     """A base class for the signed part of TUF metadata.
@@ -611,186 +604,14 @@
         """
         if reference_time is None:
             reference_time = datetime.utcnow()
 
         return reference_time >= self.expires
 
 
-class Key:
-    """A container class representing the public portion of a Key.
-
-    Supported key content (type, scheme and keyval) is defined in
-    `` Securesystemslib``.
-
-    *All parameters named below are not just constructor arguments but also
-    instance attributes.*
-
-    Args:
-        keyid: Key identifier that is unique within the metadata it is used in.
-            Keyid is not verified to be the hash of a specific representation
-            of the key.
-        keytype: Key type, e.g. "rsa", "ed25519" or "ecdsa-sha2-nistp256".
-        scheme: Signature scheme. For example:
-            "rsassa-pss-sha256", "ed25519", and "ecdsa-sha2-nistp256".
-        keyval: Opaque key content
-        unrecognized_fields: Dictionary of all attributes that are not managed
-            by TUF Metadata API
-
-    Raises:
-        TypeError: Invalid type for an argument.
-    """
-
-    def __init__(
-        self,
-        keyid: str,
-        keytype: str,
-        scheme: str,
-        keyval: Dict[str, str],
-        unrecognized_fields: Optional[Dict[str, Any]] = None,
-    ):
-        if not all(
-            isinstance(at, str) for at in [keyid, keytype, scheme]
-        ) or not isinstance(keyval, dict):
-            raise TypeError("Unexpected Key attributes types!")
-        self.keyid = keyid
-        self.keytype = keytype
-        self.scheme = scheme
-        self.keyval = keyval
-        if unrecognized_fields is None:
-            unrecognized_fields = {}
-
-        self.unrecognized_fields = unrecognized_fields
-
-    def __eq__(self, other: Any) -> bool:
-        if not isinstance(other, Key):
-            return False
-
-        return (
-            self.keyid == other.keyid
-            and self.keytype == other.keytype
-            and self.scheme == other.scheme
-            and self.keyval == other.keyval
-            and self.unrecognized_fields == other.unrecognized_fields
-        )
-
-    @classmethod
-    def from_dict(cls, keyid: str, key_dict: Dict[str, Any]) -> "Key":
-        """Create ``Key`` object from its json/dict representation.
-
-        Raises:
-            KeyError, TypeError: Invalid arguments.
-        """
-        keytype = key_dict.pop("keytype")
-        scheme = key_dict.pop("scheme")
-        keyval = key_dict.pop("keyval")
-        # All fields left in the key_dict are unrecognized.
-        return cls(keyid, keytype, scheme, keyval, key_dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of self."""
-        return {
-            "keytype": self.keytype,
-            "scheme": self.scheme,
-            "keyval": self.keyval,
-            **self.unrecognized_fields,
-        }
-
-    def to_securesystemslib_key(self) -> Dict[str, Any]:
-        """Return a ``Securesystemslib`` compatible representation of self."""
-        return {
-            "keyid": self.keyid,
-            "keytype": self.keytype,
-            "scheme": self.scheme,
-            "keyval": self.keyval,
-        }
-
-    @classmethod
-    def from_securesystemslib_key(cls, key_dict: Dict[str, Any]) -> "Key":
-        """Create a ``Key`` object from a securesystemlib key json/dict representation
-        removing the private key from keyval.
-
-        Args:
-            key_dict: Key in securesystemlib dict representation.
-
-        Raises:
-            ValueError: ``key_dict`` value is not following the securesystemslib
-                format.
-        """
-        try:
-            key_meta = sslib_keys.format_keyval_to_metadata(
-                key_dict["keytype"],
-                key_dict["scheme"],
-                key_dict["keyval"],
-            )
-        except sslib_exceptions.FormatError as e:
-            raise ValueError(
-                "key_dict value is not following the securesystemslib format"
-            ) from e
-
-        return cls(
-            key_dict["keyid"],
-            key_meta["keytype"],
-            key_meta["scheme"],
-            key_meta["keyval"],
-        )
-
-    def verify_signature(
-        self,
-        metadata: Metadata,
-        signed_serializer: Optional[SignedSerializer] = None,
-    ) -> None:
-        """Verify that the ``metadata.signatures`` contains a signature made
-        with this key, correctly signing ``metadata.signed``.
-
-        Args:
-            metadata: Metadata to verify
-            signed_serializer: ``SignedSerializer`` to serialize
-                ``metadata.signed`` with. Default is ``CanonicalJSONSerializer``.
-
-        Raises:
-            UnsignedMetadataError: The signature could not be verified for a
-                variety of possible reasons: see error message.
-        """
-        try:
-            signature = metadata.signatures[self.keyid]
-        except KeyError:
-            raise exceptions.UnsignedMetadataError(
-                f"No signature for key {self.keyid} found in metadata"
-            ) from None
-
-        if signed_serializer is None:
-            # pylint: disable=import-outside-toplevel
-            from tuf.api.serialization.json import CanonicalJSONSerializer
-
-            signed_serializer = CanonicalJSONSerializer()
-
-        try:
-            if not sslib_keys.verify_signature(
-                self.to_securesystemslib_key(),
-                signature.to_dict(),
-                signed_serializer.serialize(metadata.signed),
-            ):
-                raise exceptions.UnsignedMetadataError(
-                    f"Failed to verify {self.keyid} signature"
-                )
-        except (
-            sslib_exceptions.CryptoError,
-            sslib_exceptions.FormatError,
-            sslib_exceptions.UnsupportedAlgorithmError,
-            SerializationError,
-        ) as e:
-            # Log unexpected failure, but continue as if there was no signature
-            logger.warning(
-                "Key %s failed to verify sig: %s", self.keyid, str(e)
-            )
-            raise exceptions.UnsignedMetadataError(
-                f"Failed to verify {self.keyid} signature"
-            ) from e
-
-
 class Role:
     """Container that defines which keys are required to sign roles metadata.
 
     Role defines how many keys are required to successfully sign the roles
     metadata, and which keys are accepted.
 
     *All parameters named below are not just constructor arguments but also
@@ -989,14 +810,34 @@
         self.roles[role].keyids.remove(keyid)
         for keyinfo in self.roles.values():
             if keyid in keyinfo.keyids:
                 return
 
         del self.keys[keyid]
 
+    def get_delegated_role(self, delegated_role: str) -> Role:
+        """Return the role object for the given delegated role.
+
+        Raises ValueError if delegated_role is not actually delegated.
+        """
+        if delegated_role not in self.roles:
+            raise ValueError(f"Delegated role {delegated_role} not found")
+
+        return self.roles[delegated_role]
+
+    def get_key(self, keyid: str) -> Key:
+        """Return the key object for the given keyid.
+
+        Raises ValueError if key is not found.
+        """
+        if keyid not in self.keys:
+            raise ValueError(f"Key {keyid} not found")
+
+        return self.keys[keyid]
+
 
 class BaseFile:
     """A base class of ``MetaFile`` and ``TargetFile``.
 
     Encapsulates common static methods for length and hash verification.
     """
 
@@ -1014,21 +855,21 @@
                 else:
                     # if data is not bytes, assume it is a file object
                     digest_object = sslib_hash.digest_fileobject(data, algo)
             except (
                 sslib_exceptions.UnsupportedAlgorithmError,
                 sslib_exceptions.FormatError,
             ) as e:
-                raise exceptions.LengthOrHashMismatchError(
+                raise LengthOrHashMismatchError(
                     f"Unsupported algorithm '{algo}'"
                 ) from e
 
             observed_hash = digest_object.hexdigest()
             if observed_hash != exp_hash:
-                raise exceptions.LengthOrHashMismatchError(
+                raise LengthOrHashMismatchError(
                     f"Observed hash {observed_hash} does not match "
                     f"expected hash {exp_hash}"
                 )
 
     @staticmethod
     def _verify_length(
         data: Union[bytes, IO[bytes]], expected_length: int
@@ -1038,15 +879,15 @@
             observed_length = len(data)
         else:
             # if data is not bytes, assume it is a file object
             data.seek(0, io.SEEK_END)
             observed_length = data.tell()
 
         if observed_length != expected_length:
-            raise exceptions.LengthOrHashMismatchError(
+            raise LengthOrHashMismatchError(
                 f"Observed length {observed_length} does not match "
                 f"expected length {expected_length}"
             )
 
     @staticmethod
     def _validate_hashes(hashes: Dict[str, str]) -> None:
         if not hashes:
@@ -1082,15 +923,14 @@
     def __init__(
         self,
         version: int = 1,
         length: Optional[int] = None,
         hashes: Optional[Dict[str, str]] = None,
         unrecognized_fields: Optional[Dict[str, Any]] = None,
     ):
-
         if version <= 0:
             raise ValueError(f"Metafile version must be > 0, got {version}")
         if length is not None:
             self._validate_length(length)
         if hashes is not None:
             self._validate_hashes(hashes)
 
@@ -1756,30 +1596,31 @@
     def __init__(
         self,
         length: int,
         hashes: Dict[str, str],
         path: str,
         unrecognized_fields: Optional[Dict[str, Any]] = None,
     ):
-
         self._validate_length(length)
         self._validate_hashes(hashes)
 
         self.length = length
         self.hashes = hashes
         self.path = path
         if unrecognized_fields is None:
             unrecognized_fields = {}
 
         self.unrecognized_fields = unrecognized_fields
 
     @property
     def custom(self) -> Any:
-        """Can be used to provide implementation specific data related to the
-        target. python-tuf does not use or validate this data."""
+        """Get implementation specific data related to the target.
+
+        python-tuf does not use or validate this data.
+        """
         return self.unrecognized_fields.get("custom")
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, TargetFile):
             return False
 
         return (
@@ -1892,14 +1733,25 @@
         Raises:
             LengthOrHashMismatchError: Calculated length or hashes do not
                 match expected values or hash algorithm is not supported.
         """
         self._verify_length(data, self.length)
         self._verify_hashes(data, self.hashes)
 
+    def get_prefixed_paths(self) -> List[str]:
+        """
+        Return hash-prefixed URL path fragments for the target file path.
+        """
+        paths = []
+        parent, sep, name = self.path.rpartition("/")
+        for hash_value in self.hashes.values():
+            paths.append(f"{parent}{sep}{hash_value}.{name}")
+
+        return paths
+
 
 class Targets(Signed):
     """A container for the signed part of targets metadata.
 
     Targets contains verifying information about target files and also
     delegates responsibility to other Targets roles.
 
@@ -2048,7 +1900,37 @@
                 raise ValueError(
                     f"Key with id {keyid} is not used by succinct_roles"
                 )
 
             self.delegations.succinct_roles.keyids.remove(keyid)
 
         del self.delegations.keys[keyid]
+
+    def get_delegated_role(self, delegated_role: str) -> Role:
+        """Return the role object for the given delegated role.
+
+        Raises ValueError if delegated_role is not actually delegated.
+        """
+        if self.delegations is None:
+            raise ValueError("No delegations found")
+
+        if self.delegations.roles is not None:
+            role: Optional[Role] = self.delegations.roles.get(delegated_role)
+        else:
+            role = self.delegations.succinct_roles
+
+        if not role:
+            raise ValueError(f"Delegated role {delegated_role} not found")
+
+        return role
+
+    def get_key(self, keyid: str) -> Key:
+        """Return the key object for the given keyid.
+
+        Raises ValueError if keyid is not found.
+        """
+        if self.delegations is None:
+            raise ValueError("No delegations found")
+        if keyid not in self.delegations.keys:
+            raise ValueError(f"Key {keyid} not found")
+
+        return self.delegations.keys[keyid]
```

### Comparing `tuf-2.1.0/tuf/api/serialization/__init__.py` & `tuf-3.0.0/tuf/api/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tuf/api/serialization/json.py` & `tuf-3.0.0/tuf/api/serialization/json.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tuf/ngclient/README.md` & `tuf-3.0.0/tuf/ngclient/README.md`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tuf/ngclient/__init__.py` & `tuf-3.0.0/tuf/ngclient/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Copyright New York University and the TUF contributors
 # SPDX-License-Identifier: MIT OR Apache-2.0
 
 """TUF client public API.
 """
 
 
+from tuf.api.metadata import TargetFile
+
 # requests_fetcher is public but comes from _internal for now (because
 # sigstore-python 1.0 still uses the module from there). requests_fetcher
 # can be moved out of _internal once sigstore-python 1.0 is not relevant.
 from tuf.ngclient._internal.requests_fetcher import RequestsFetcher
 from tuf.ngclient.config import UpdaterConfig
 from tuf.ngclient.fetcher import FetcherInterface
 from tuf.ngclient.updater import Updater
 
 __all__ = [
     FetcherInterface.__name__,
     RequestsFetcher.__name__,
+    TargetFile.__name__,
     Updater.__name__,
     UpdaterConfig.__name__,
 ]
```

### Comparing `tuf-2.1.0/tuf/ngclient/config.py` & `tuf-3.0.0/tuf/ngclient/config.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tuf/ngclient/fetcher.py` & `tuf-3.0.0/tuf/ngclient/fetcher.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tuf/ngclient/updater.py` & `tuf-3.0.0/tuf/ngclient/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         verified correct by the metadata.
 
 Note that applications using ``Updater`` should be 'single instance'
 applications: running multiple instances that use the same cache directories at
 the same time is not supported.
 
 A simple example of using the Updater to implement a Python TUF client that
-downloads target files is available in `examples/client_example
-<https://github.com/theupdateframework/python-tuf/tree/develop/examples/client_example>`_.
+downloads target files is available in `examples/client
+<https://github.com/theupdateframework/python-tuf/tree/develop/examples/client>`_.
 """
 
 import logging
 import os
 import shutil
 import tempfile
 from typing import Optional, Set
@@ -424,15 +424,14 @@
         visited_role_names: Set[str] = set()
 
         # Preorder depth-first traversal of the graph of target delegations.
         while (
             len(visited_role_names) <= self.config.max_delegations
             and len(delegations_to_visit) > 0
         ):
-
             # Pop the role name from the top of the stack.
             role_name, parent_role = delegations_to_visit.pop(-1)
 
             # Skip any visited current role to prevent cycles.
             if role_name in visited_role_names:
                 logger.debug("Skipping visited current role %s", role_name)
                 continue
@@ -454,15 +453,14 @@
                 child_roles_to_visit = []
                 # NOTE: This may be a slow operation if there are many
                 # delegated roles.
                 for (
                     child_name,
                     terminating,
                 ) in targets.delegations.get_roles_for_target(target_filepath):
-
                     logger.debug("Adding child role %s", child_name)
                     child_roles_to_visit.append((child_name, role_name))
                     if terminating:
                         logger.debug("Not backtracking to other roles")
                         delegations_to_visit = []
                         break
                 # Push 'child_roles_to_visit' in reverse order of appearance
```

### Comparing `tuf-2.1.0/tuf/ngclient/_internal/requests_fetcher.py` & `tuf-3.0.0/tuf/ngclient/_internal/requests_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import tuf
 from tuf.api import exceptions
 from tuf.ngclient.fetcher import FetcherInterface
 
 # Globals
 logger = logging.getLogger(__name__)
 
+
 # Classes
 class RequestsFetcher(FetcherInterface):
     """An implementation of ``FetcherInterface`` based on the requests library.
 
     Attributes:
         socket_timeout: Timeout in seconds, used for both initial connection
             delay and the maximum delay between bytes received. Default is
@@ -92,17 +93,19 @@
             response.close()
             status = e.response.status_code
             raise exceptions.DownloadHTTPError(str(e), status)
 
         return self._chunks(response)
 
     def _chunks(self, response: "requests.Response") -> Iterator[bytes]:
-        """A generator function to be returned by fetch. This way the
-        caller of fetch can differentiate between connection and actual data
-        download."""
+        """A generator function to be returned by fetch.
+
+        This way the caller of fetch can differentiate between connection
+        and actual data download.
+        """
 
         try:
             for data in response.iter_content(self.chunk_size):
                 yield data
         except (
             requests.exceptions.ConnectionError,
             requests.exceptions.Timeout,
```

### Comparing `tuf-2.1.0/tuf/ngclient/_internal/trusted_metadata_set.py` & `tuf-3.0.0/tuf/ngclient/_internal/trusted_metadata_set.py`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/tuf/repository/_repository.py` & `tuf-3.0.0/tuf/repository/_repository.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 
 import logging
 from abc import ABC, abstractmethod
 from contextlib import contextmanager, suppress
 from copy import deepcopy
 from typing import Dict, Generator, Optional, Tuple
 
-from tuf.api.metadata import Metadata, MetaFile, Signed
+from tuf.api.metadata import (
+    Metadata,
+    MetaFile,
+    Root,
+    Signed,
+    Snapshot,
+    Targets,
+    Timestamp,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class AbortEdit(Exception):
     """Raise to exit the edit() contextmanager without saving changes"""
 
@@ -36,45 +44,49 @@
     in this base class.
     """
 
     @abstractmethod
     def open(self, role: str) -> Metadata:
         """Load a roles metadata from storage or cache, return it
 
-        If role has no metadata, create first version from scratch"""
+        If role has no metadata, create first version from scratch.
+        """
         raise NotImplementedError
 
     @abstractmethod
     def close(self, role: str, md: Metadata) -> None:
         """Write roles metadata into storage
 
         Update expiry and version and replace signatures with ones from all
-        available keys. Keep snapshot_info and targets_infos updated."""
+        available keys. Keep snapshot_info and targets_infos updated.
+        """
         raise NotImplementedError
 
     @property
-    @abstractmethod
     def targets_infos(self) -> Dict[str, MetaFile]:
         """Returns the MetaFiles for current targets metadatas
 
-        This property is used by snapshot() to update Snapshot.meta.
+        This property is used by do_snapshot() to update Snapshot.meta:
+        Repository implementations should override this property to enable
+        do_snapshot().
 
         Note that there is a difference between this return value and
         Snapshot.meta: This dictionary reflects the targets metadata that
         currently exists in the repository but Snapshot.meta also includes
         metadata that used to exist, but no longer exists, in the repository.
         """
         raise NotImplementedError
 
     @property
-    @abstractmethod
     def snapshot_info(self) -> MetaFile:
         """Returns the MetaFile for current snapshot metadata
 
-        This property is used by timestamp() to update Timestamp.meta.
+        This property is used by do_timestamp() to update Timestamp.meta:
+        Repository implementations should override this property to enable
+        do_timestamp().
         """
         raise NotImplementedError
 
     @contextmanager
     def edit(self, role: str) -> Generator[Signed, None, None]:
         """Context manager for editing a role's metadata
 
@@ -87,15 +99,79 @@
         cancel the edit: in this case none of the changes are stored.
         """
         md = self.open(role)
         with suppress(AbortEdit):
             yield md.signed
             self.close(role, md)
 
-    def snapshot(self, force: bool = False) -> Tuple[bool, Dict[str, MetaFile]]:
+    @contextmanager
+    def edit_root(self) -> Generator[Root, None, None]:
+        """Context manager for editing root metadata. See edit()"""
+        with self.edit(Root.type) as root:
+            if not isinstance(root, Root):
+                raise RuntimeError("Unexpected root type")
+            yield root
+
+    @contextmanager
+    def edit_timestamp(self) -> Generator[Timestamp, None, None]:
+        """Context manager for editing timestamp metadata. See edit()"""
+        with self.edit(Timestamp.type) as timestamp:
+            if not isinstance(timestamp, Timestamp):
+                raise RuntimeError("Unexpected timestamp type")
+            yield timestamp
+
+    @contextmanager
+    def edit_snapshot(self) -> Generator[Snapshot, None, None]:
+        """Context manager for editing snapshot metadata. See edit()"""
+        with self.edit(Snapshot.type) as snapshot:
+            if not isinstance(snapshot, Snapshot):
+                raise RuntimeError("Unexpected snapshot type")
+            yield snapshot
+
+    @contextmanager
+    def edit_targets(
+        self, rolename: str = Targets.type
+    ) -> Generator[Targets, None, None]:
+        """Context manager for editing targets metadata. See edit()"""
+        with self.edit(rolename) as targets:
+            if not isinstance(targets, Targets):
+                raise RuntimeError(f"Unexpected targets ({rolename}) type")
+            yield targets
+
+    def root(self) -> Root:
+        """Read current root metadata"""
+        root = self.open(Root.type).signed
+        if not isinstance(root, Root):
+            raise RuntimeError("Unexpected root type")
+        return root
+
+    def timestamp(self) -> Timestamp:
+        """Read current timestamp metadata"""
+        timestamp = self.open(Timestamp.type).signed
+        if not isinstance(timestamp, Timestamp):
+            raise RuntimeError("Unexpected timestamp type")
+        return timestamp
+
+    def snapshot(self) -> Snapshot:
+        """Read current snapshot metadata"""
+        snapshot = self.open(Snapshot.type).signed
+        if not isinstance(snapshot, Snapshot):
+            raise RuntimeError("Unexpected snapshot type")
+        return snapshot
+
+    def targets(self, rolename: str = Targets.type) -> Targets:
+        """Read current targets metadata"""
+        targets = self.open(rolename).signed
+        if not isinstance(targets, Targets):
+            raise RuntimeError("Unexpected targets type")
+        return targets
+
+    def do_snapshot(
+        self, force: bool = False
+    ) -> Tuple[bool, Dict[str, MetaFile]]:
         """Update snapshot meta information
 
         Updates the snapshot meta information according to current targets
         metadata state and the current snapshot meta information.
 
         Arguments:
             force: should new snapshot version be created even if meta
@@ -108,15 +184,15 @@
 
         # Snapshot update is needed if
         # * any targets files are not yet in snapshot or
         # * any targets version is incorrect
         update_version = force
         removed: Dict[str, MetaFile] = {}
 
-        with self.edit("snapshot") as snapshot:
+        with self.edit_snapshot() as snapshot:
             for keyname, new_meta in self.targets_infos.items():
                 if keyname not in snapshot.meta:
                     update_version = True
                     snapshot.meta[keyname] = deepcopy(new_meta)
                     continue
 
                 old_meta = snapshot.meta[keyname]
@@ -124,47 +200,49 @@
                     raise ValueError(f"{keyname} version rollback")
                 if new_meta.version > old_meta.version:
                     update_version = True
                     snapshot.meta[keyname] = deepcopy(new_meta)
                     removed[keyname] = old_meta
 
             if not update_version:
-                # prevent edit() from storing a new snapshot version
+                # prevent edit_snapshot() from storing a new version
                 raise AbortEdit("Skip snapshot: No targets version changes")
 
         if not update_version:
-            # this is reachable as edit() handles AbortEdit
+            # this is reachable as edit_snapshot() handles AbortEdit
             logger.debug("Snapshot update not needed")  # type: ignore[unreachable]
         else:
             logger.debug("Snapshot v%d", snapshot.version)
 
         return update_version, removed
 
-    def timestamp(self, force: bool = False) -> Tuple[bool, Optional[MetaFile]]:
+    def do_timestamp(
+        self, force: bool = False
+    ) -> Tuple[bool, Optional[MetaFile]]:
         """Update timestamp meta information
 
         Updates timestamp according to current snapshot state
 
         Returns: Tuple of
             - True if timestamp was created, False if not
             - MetaFile for snapshot version removed from timestamp (if any)
         """
         update_version = force
         removed = None
-        with self.edit("timestamp") as timestamp:
+        with self.edit_timestamp() as timestamp:
             if self.snapshot_info.version < timestamp.snapshot_meta.version:
                 raise ValueError("snapshot version rollback")
 
             if self.snapshot_info.version > timestamp.snapshot_meta.version:
                 update_version = True
                 removed = timestamp.snapshot_meta
                 timestamp.snapshot_meta = deepcopy(self.snapshot_info)
 
             if not update_version:
                 raise AbortEdit("Skip timestamp: No snapshot version changes")
 
         if not update_version:
-            # this is reachable as edit() handles AbortEdit
+            # this is reachable as edit_timestamp() handles AbortEdit
             logger.debug("Timestamp update not needed")  # type: ignore[unreachable]
         else:
             logger.debug("Timestamp v%d", timestamp.version)
         return update_version, removed
```

### Comparing `tuf-2.1.0/LICENSE` & `tuf-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/LICENSE-MIT` & `tuf-3.0.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `tuf-2.1.0/README.md` & `tuf-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 [The Update Framework (TUF)](https://theupdateframework.io/) is a framework for
 secure content delivery and updates. It protects against various types of
 supply chain attacks and provides resilience to compromise. This repository is a
 **reference implementation** written in Python. It is intended to conform to
 version 1.0 of the [TUF
 specification](https://theupdateframework.github.io/specification/latest/).
 
-Python-TUF provides two APIs:
+Python-TUF provides the following APIs:
   * [`tuf.api.metadata`](https://theupdateframework.readthedocs.io/en/latest/api/tuf.api.html),
     a "low-level" API, designed to provide easy and safe access to TUF
     metadata and to handle (de)serialization from/to files.
   * [`tuf.ngclient`](https://theupdateframework.readthedocs.io/en/latest/api/tuf.ngclient.html),
     a client implementation built on top of the metadata API.
-
-High-level support for implementing
-[repository operations](https://theupdateframework.github.io/specification/latest/#repository-operations)
-is planned but not yet provided: see [ADR 10](https://github.com/theupdateframework/python-tuf/blob/develop/docs/adr/0010-repository-library-design.md).
+  * `tuf.repository`, a repository library also built on top of the metadata
+    API. This module is currently not considered part of python-tuf stable API.
 
 The reference implementation strives to be a readable guide and demonstration
 for those working on implementing TUF in their own languages, environments, or
 update systems.
 
 
 About The Update Framework
```

### Comparing `tuf-2.1.0/pyproject.toml` & `tuf-3.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 # hatchling pinned for reproducibility: version should be kept up-to-date
-requires = ["hatchling==1.11.1"]
+requires = ["hatchling==1.13.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tuf"
 description = "A secure updater framework for Python"
 readme = "README.md"
 license = { text = "MIT OR Apache-2.0" }
@@ -40,15 +40,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Security",
   "Topic :: Software Development",
 ]
 dependencies = [
   "requests>=2.19.1",
-  "securesystemslib>=0.22.0",
+  "securesystemslib>=0.26.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://theupdateframework.readthedocs.io/en/stable/"
 Homepage = "https://www.updateframework.com"
 Issues = "https://github.com/theupdateframework/python-tuf/issues"
@@ -59,15 +59,15 @@
 
 [tool.hatch.build.targets.sdist]
 include = [
   "/docs",
   "/examples",
   "/tests",
   "/tuf",
-  "/requirements*.txt",
+  "/requirements",
   "/tox.ini",
   "/setup.py",
 ]
 
 [tool.hatch.build.targets.wheel]
 # The testing phase changes the current working directory to `tests` but the test scripts import
 # from `tests` so the root directory must be added to Python's path for editable installations
@@ -150,7 +150,11 @@
 
 [[tool.mypy.overrides]]
 module = [
   "requests.*",
   "securesystemslib.*",
 ]
 ignore_missing_imports = "True"
+
+[tool.pydocstyle]
+inherit = false
+ignore = "D400,D415,D213,D205,D202,D107,D407,D413,D212,D104,D406,D105,D411,D401,D200,D203"
```

### Comparing `tuf-2.1.0/PKG-INFO` & `tuf-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuf
-Version: 2.1.0
+Version: 3.0.0
 Summary: A secure updater framework for Python
 Project-URL: Documentation, https://theupdateframework.readthedocs.io/en/stable/
 Project-URL: Homepage, https://www.updateframework.com
 Project-URL: Issues, https://github.com/theupdateframework/python-tuf/issues
 Project-URL: Source, https://github.com/theupdateframework/python-tuf
 Author-email: theupdateframework@googlegroups.com
 License: MIT OR Apache-2.0
@@ -28,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Requires-Dist: requests>=2.19.1
-Requires-Dist: securesystemslib>=0.22.0
+Requires-Dist: securesystemslib>=0.26.0
 Description-Content-Type: text/markdown
 
 # <img src="https://cdn.rawgit.com/theupdateframework/artwork/3a649fa6/tuf-logo.svg" height="100" valign="middle" alt="TUF"/> A Framework for Securing Software Update Systems
 
 ![Build](https://github.com/theupdateframework/python-tuf/actions/workflows/ci.yml/badge.svg)
 [![Coveralls](https://coveralls.io/repos/theupdateframework/python-tuf/badge.svg?branch=develop)](https://coveralls.io/r/theupdateframework/python-tuf?branch=develop)
 [![Docs](https://readthedocs.org/projects/theupdateframework/badge/)](https://theupdateframework.readthedocs.io/)
@@ -48,24 +48,22 @@
 [The Update Framework (TUF)](https://theupdateframework.io/) is a framework for
 secure content delivery and updates. It protects against various types of
 supply chain attacks and provides resilience to compromise. This repository is a
 **reference implementation** written in Python. It is intended to conform to
 version 1.0 of the [TUF
 specification](https://theupdateframework.github.io/specification/latest/).
 
-Python-TUF provides two APIs:
+Python-TUF provides the following APIs:
   * [`tuf.api.metadata`](https://theupdateframework.readthedocs.io/en/latest/api/tuf.api.html),
     a "low-level" API, designed to provide easy and safe access to TUF
     metadata and to handle (de)serialization from/to files.
   * [`tuf.ngclient`](https://theupdateframework.readthedocs.io/en/latest/api/tuf.ngclient.html),
     a client implementation built on top of the metadata API.
-
-High-level support for implementing
-[repository operations](https://theupdateframework.github.io/specification/latest/#repository-operations)
-is planned but not yet provided: see [ADR 10](https://github.com/theupdateframework/python-tuf/blob/develop/docs/adr/0010-repository-library-design.md).
+  * `tuf.repository`, a repository library also built on top of the metadata
+    API. This module is currently not considered part of python-tuf stable API.
 
 The reference implementation strives to be a readable guide and demonstration
 for those working on implementing TUF in their own languages, environments, or
 update systems.
 
 
 About The Update Framework
```

