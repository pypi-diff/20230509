# Comparing `tmp/gradio_tools-0.0.7.tar.gz` & `tmp/gradio_tools-0.0.8.tar.gz`

## Comparing `gradio_tools-0.0.7.tar` & `gradio_tools-0.0.8.tar`

### file list

```diff
@@ -1,148 +1,154 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/.DS_Store
--rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/README.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/passwords.txt
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/temp.log
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/.vscode/settings.json
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/162952a0-7147-4f52-ab58-f852bc5c0561/captions.json
--rw-r--r--   0        0        0   109150 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg
--rw-r--r--   0        0        0    79996 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg
--rw-r--r--   0        0        0    99128 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg
--rw-r--r--   0        0        0   101966 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/captions.json
--rw-r--r--   0        0        0   143165 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpd4fe9ahm.jpg
--rw-r--r--   0        0        0    97772 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpe0qa0lhx.jpg
--rw-r--r--   0        0        0    94365 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpnvmcs9su.jpg
--rw-r--r--   0        0        0    71624 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpwvlf4c_7.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/27195f48-ea83-46b0-be72-39e76f1432a3/captions.json
--rw-r--r--   0        0        0   140326 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/27195f48-ea83-46b0-be72-39e76f1432a3/tmp0364mijl.jpg
--rw-r--r--   0        0        0    63032 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/27195f48-ea83-46b0-be72-39e76f1432a3/tmpn8vk75sg.jpg
--rw-r--r--   0        0        0    90188 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/27195f48-ea83-46b0-be72-39e76f1432a3/tmpp4x_v2hp.jpg
--rw-r--r--   0        0        0   139229 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/27195f48-ea83-46b0-be72-39e76f1432a3/tmpvswx2fg1.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/captions.json
--rw-r--r--   0        0        0   123839 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp37n48nis.jpg
--rw-r--r--   0        0        0    74284 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp6_fdz6c8.jpg
--rw-r--r--   0        0        0   110328 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp_kkj0za7.jpg
--rw-r--r--   0        0        0   110178 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmpbjq5o1s2.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/330d40a3-cc6a-41ce-96c2-002bc67df326/captions.json
--rw-r--r--   0        0        0   105846 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg
--rw-r--r--   0        0        0   126760 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg
--rw-r--r--   0        0        0   119178 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg
--rw-r--r--   0        0        0   108581 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/captions.json
--rw-r--r--   0        0        0    99607 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg
--rw-r--r--   0        0        0   131260 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg
--rw-r--r--   0        0        0   116900 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg
--rw-r--r--   0        0        0    80104 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/508529be-bc20-48b9-b0b7-003e7a21db62/captions.json
--rw-r--r--   0        0        0   122753 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg
--rw-r--r--   0        0        0    86812 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg
--rw-r--r--   0        0        0   105885 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg
--rw-r--r--   0        0        0   117917 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/captions.json
--rw-r--r--   0        0        0   106965 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpmsy7r5s4.jpg
--rw-r--r--   0        0        0   126635 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpotr65fvw.jpg
--rw-r--r--   0        0        0   103678 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpr4__qxcx.jpg
--rw-r--r--   0        0        0    94221 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpx4p7b1ft.jpg
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/5b6efdad-3ce5-4de9-a2b6-ded17b234523/captions.json
--rw-r--r--   0        0        0   141280 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmpjumozfel.jpg
--rw-r--r--   0        0        0   111566 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmppfkjroq_.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/6a6c3f15-5217-462c-9d28-39f1b2f07676/captions.json
--rw-r--r--   0        0        0   135053 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpj6tqr3fx.jpg
--rw-r--r--   0        0        0   108105 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpodtfruna.jpg
--rw-r--r--   0        0        0   137541 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmppg3kuayo.jpg
--rw-r--r--   0        0        0   103154 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmps600nxhc.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/70a06453-f83c-4866-89a1-d8f5c9a052d7/captions.json
--rw-r--r--   0        0        0    77205 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg
--rw-r--r--   0        0        0    92290 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg
--rw-r--r--   0        0        0   120803 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg
--rw-r--r--   0        0        0    89928 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/captions.json
--rw-r--r--   0        0        0    99904 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmp0bq293n9.jpg
--rw-r--r--   0        0        0    75479 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmphhgdi5d9.jpg
--rw-r--r--   0        0        0    96797 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmpjgndeko_.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/75c113a2-7d4f-4f14-abe9-23259df50dfb/captions.json
--rw-r--r--   0        0        0    96910 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg
--rw-r--r--   0        0        0    81978 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg
--rw-r--r--   0        0        0   112268 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg
--rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/captions.json
--rw-r--r--   0        0        0    93851 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmp74tk8cfs.jpg
--rw-r--r--   0        0        0   115711 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpk_wbbklr.jpg
--rw-r--r--   0        0        0    89571 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpvufkgo26.jpg
--rw-r--r--   0        0        0   112338 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpz6lir7im.jpg
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/captions.json
--rw-r--r--   0        0        0    47561 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpnu2s0p5c.jpg
--rw-r--r--   0        0        0   104221 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpsvafzhhw.jpg
--rw-r--r--   0        0        0    73088 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpx8aicgye.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa3ee281-8672-4993-bb3e-09335e1de70e/captions.json
--rw-r--r--   0        0        0   122186 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg
--rw-r--r--   0        0        0    93863 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg
--rw-r--r--   0        0        0   121362 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg
--rw-r--r--   0        0        0    80154 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa9874d1-dc09-4c04-bf37-55c556e61e83/captions.json
--rw-r--r--   0        0        0   111564 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmp5myeybsm.jpg
--rw-r--r--   0        0        0    98332 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpd3ufb_2o.jpg
--rw-r--r--   0        0        0   112096 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpdlfj8cj_.jpg
--rw-r--r--   0        0        0   109146 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmps0tx8a8q.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ac2f6e03-9430-4c22-a559-354225a49357/captions.json
--rw-r--r--   0        0        0    79381 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg
--rw-r--r--   0        0        0   105896 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg
--rw-r--r--   0        0        0    92696 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg
--rw-r--r--   0        0        0   112587 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/captions.json
--rw-r--r--   0        0        0   103101 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpg2htn2w7.jpg
--rw-r--r--   0        0        0    81958 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpkoqyldk0.jpg
--rw-r--r--   0        0        0    55884 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpnru9hk2q.jpg
--rw-r--r--   0        0        0    83078 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpvxkwhzbo.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/captions.json
--rw-r--r--   0        0        0    93651 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmp7n9_771q.jpg
--rw-r--r--   0        0        0    83077 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpgaejg5rz.jpg
--rw-r--r--   0        0        0   101925 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpl3n0u99v.jpg
--rw-r--r--   0        0        0   122576 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpuylgwvrf.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d52f969d-6985-461d-bf02-080c86e36628/captions.json
--rw-r--r--   0        0        0   133445 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d52f969d-6985-461d-bf02-080c86e36628/tmpe6rm8dhh.jpg
--rw-r--r--   0        0        0    76358 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d52f969d-6985-461d-bf02-080c86e36628/tmpk6ugfnjb.jpg
--rw-r--r--   0        0        0    67170 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d52f969d-6985-461d-bf02-080c86e36628/tmpnmfnsc82.jpg
--rw-r--r--   0        0        0    79654 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/d52f969d-6985-461d-bf02-080c86e36628/tmpy8mg_mm2.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/captions.json
--rw-r--r--   0        0        0    99572 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmphp1_2bwe.jpg
--rw-r--r--   0        0        0   115349 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmplv4pugrr.jpg
--rw-r--r--   0        0        0    91136 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpsvh8rgjz.jpg
--rw-r--r--   0        0        0    91363 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpvtinxpmw.jpg
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/langchain/bark_example.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/langchain/document_qa.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/langchain/example.py
--rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/langchain/florida-drivers-license.jpeg
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/langchain/sam_example.py
--rw-r--r--   0        0        0   209515 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/langchain/waldo.jpeg
--rw-r--r--   0        0        0   263388 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/langchain/waldo_3.webp
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/minichain/agent.pmpt.tpl
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/minichain/agent.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/examples/minichain/example.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/__init__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/__init__.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/bark.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/clip_interrogator.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/document_qa.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/gradio_tool.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/image_captioning.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/image_to_music.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/prompt_generator.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/sam_with_clip.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/stable_diffusion.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/text_to_video.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/gradio_tools/tools/whisper.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/scripts/format.sh
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/scripts/lint.sh
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/tests/test_sam.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/tests/test_tools.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/LICENSE
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8667 2020-02-02 00:00:00.000000 gradio_tools-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/.DS_Store
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/README.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/passwords.txt
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/plugin_py.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/temp.log
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/042cc880-66df-4bcf-9018-af0b42d131ad/captions.json
+-rw-r--r--   0        0        0   101356 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/042cc880-66df-4bcf-9018-af0b42d131ad/tmp3aun5q6h.jpg
+-rw-r--r--   0        0        0   127532 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/042cc880-66df-4bcf-9018-af0b42d131ad/tmp97l2_5jd.jpg
+-rw-r--r--   0        0        0   111221 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/042cc880-66df-4bcf-9018-af0b42d131ad/tmpt6rkm4b5.jpg
+-rw-r--r--   0        0        0    86598 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/042cc880-66df-4bcf-9018-af0b42d131ad/tmptzlty8zj.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/162952a0-7147-4f52-ab58-f852bc5c0561/captions.json
+-rw-r--r--   0        0        0   109150 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg
+-rw-r--r--   0        0        0    79996 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg
+-rw-r--r--   0        0        0    99128 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg
+-rw-r--r--   0        0        0   101966 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/captions.json
+-rw-r--r--   0        0        0   143165 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpd4fe9ahm.jpg
+-rw-r--r--   0        0        0    97772 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpe0qa0lhx.jpg
+-rw-r--r--   0        0        0    94365 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpnvmcs9su.jpg
+-rw-r--r--   0        0        0    71624 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpwvlf4c_7.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/27195f48-ea83-46b0-be72-39e76f1432a3/captions.json
+-rw-r--r--   0        0        0   140326 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/27195f48-ea83-46b0-be72-39e76f1432a3/tmp0364mijl.jpg
+-rw-r--r--   0        0        0    63032 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/27195f48-ea83-46b0-be72-39e76f1432a3/tmpn8vk75sg.jpg
+-rw-r--r--   0        0        0    90188 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/27195f48-ea83-46b0-be72-39e76f1432a3/tmpp4x_v2hp.jpg
+-rw-r--r--   0        0        0   139229 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/27195f48-ea83-46b0-be72-39e76f1432a3/tmpvswx2fg1.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/captions.json
+-rw-r--r--   0        0        0   123839 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp37n48nis.jpg
+-rw-r--r--   0        0        0    74284 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp6_fdz6c8.jpg
+-rw-r--r--   0        0        0   110328 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp_kkj0za7.jpg
+-rw-r--r--   0        0        0   110178 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmpbjq5o1s2.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/330d40a3-cc6a-41ce-96c2-002bc67df326/captions.json
+-rw-r--r--   0        0        0   105846 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg
+-rw-r--r--   0        0        0   126760 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg
+-rw-r--r--   0        0        0   119178 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg
+-rw-r--r--   0        0        0   108581 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/captions.json
+-rw-r--r--   0        0        0    99607 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg
+-rw-r--r--   0        0        0   131260 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg
+-rw-r--r--   0        0        0   116900 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg
+-rw-r--r--   0        0        0    80104 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/508529be-bc20-48b9-b0b7-003e7a21db62/captions.json
+-rw-r--r--   0        0        0   122753 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg
+-rw-r--r--   0        0        0    86812 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg
+-rw-r--r--   0        0        0   105885 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg
+-rw-r--r--   0        0        0   117917 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/captions.json
+-rw-r--r--   0        0        0   106965 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpmsy7r5s4.jpg
+-rw-r--r--   0        0        0   126635 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpotr65fvw.jpg
+-rw-r--r--   0        0        0   103678 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpr4__qxcx.jpg
+-rw-r--r--   0        0        0    94221 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpx4p7b1ft.jpg
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/5b6efdad-3ce5-4de9-a2b6-ded17b234523/captions.json
+-rw-r--r--   0        0        0   141280 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmpjumozfel.jpg
+-rw-r--r--   0        0        0   111566 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmppfkjroq_.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/6a6c3f15-5217-462c-9d28-39f1b2f07676/captions.json
+-rw-r--r--   0        0        0   135053 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpj6tqr3fx.jpg
+-rw-r--r--   0        0        0   108105 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpodtfruna.jpg
+-rw-r--r--   0        0        0   137541 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmppg3kuayo.jpg
+-rw-r--r--   0        0        0   103154 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmps600nxhc.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/70a06453-f83c-4866-89a1-d8f5c9a052d7/captions.json
+-rw-r--r--   0        0        0    77205 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg
+-rw-r--r--   0        0        0    92290 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg
+-rw-r--r--   0        0        0   120803 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg
+-rw-r--r--   0        0        0    89928 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/captions.json
+-rw-r--r--   0        0        0    99904 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmp0bq293n9.jpg
+-rw-r--r--   0        0        0    75479 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmphhgdi5d9.jpg
+-rw-r--r--   0        0        0    96797 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmpjgndeko_.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/75c113a2-7d4f-4f14-abe9-23259df50dfb/captions.json
+-rw-r--r--   0        0        0    96910 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg
+-rw-r--r--   0        0        0    81978 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg
+-rw-r--r--   0        0        0   112268 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg
+-rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/captions.json
+-rw-r--r--   0        0        0    93851 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmp74tk8cfs.jpg
+-rw-r--r--   0        0        0   115711 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpk_wbbklr.jpg
+-rw-r--r--   0        0        0    89571 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpvufkgo26.jpg
+-rw-r--r--   0        0        0   112338 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpz6lir7im.jpg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/captions.json
+-rw-r--r--   0        0        0    47561 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpnu2s0p5c.jpg
+-rw-r--r--   0        0        0   104221 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpsvafzhhw.jpg
+-rw-r--r--   0        0        0    73088 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpx8aicgye.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa3ee281-8672-4993-bb3e-09335e1de70e/captions.json
+-rw-r--r--   0        0        0   122186 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg
+-rw-r--r--   0        0        0    93863 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg
+-rw-r--r--   0        0        0   121362 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg
+-rw-r--r--   0        0        0    80154 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa9874d1-dc09-4c04-bf37-55c556e61e83/captions.json
+-rw-r--r--   0        0        0   111564 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmp5myeybsm.jpg
+-rw-r--r--   0        0        0    98332 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpd3ufb_2o.jpg
+-rw-r--r--   0        0        0   112096 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpdlfj8cj_.jpg
+-rw-r--r--   0        0        0   109146 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmps0tx8a8q.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ac2f6e03-9430-4c22-a559-354225a49357/captions.json
+-rw-r--r--   0        0        0    79381 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg
+-rw-r--r--   0        0        0   105896 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg
+-rw-r--r--   0        0        0    92696 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg
+-rw-r--r--   0        0        0   112587 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/captions.json
+-rw-r--r--   0        0        0   103101 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpg2htn2w7.jpg
+-rw-r--r--   0        0        0    81958 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpkoqyldk0.jpg
+-rw-r--r--   0        0        0    55884 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpnru9hk2q.jpg
+-rw-r--r--   0        0        0    83078 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpvxkwhzbo.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/captions.json
+-rw-r--r--   0        0        0    93651 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmp7n9_771q.jpg
+-rw-r--r--   0        0        0    83077 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpgaejg5rz.jpg
+-rw-r--r--   0        0        0   101925 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpl3n0u99v.jpg
+-rw-r--r--   0        0        0   122576 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpuylgwvrf.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d52f969d-6985-461d-bf02-080c86e36628/captions.json
+-rw-r--r--   0        0        0   133445 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d52f969d-6985-461d-bf02-080c86e36628/tmpe6rm8dhh.jpg
+-rw-r--r--   0        0        0    76358 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d52f969d-6985-461d-bf02-080c86e36628/tmpk6ugfnjb.jpg
+-rw-r--r--   0        0        0    67170 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d52f969d-6985-461d-bf02-080c86e36628/tmpnmfnsc82.jpg
+-rw-r--r--   0        0        0    79654 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/d52f969d-6985-461d-bf02-080c86e36628/tmpy8mg_mm2.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/captions.json
+-rw-r--r--   0        0        0    99572 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmphp1_2bwe.jpg
+-rw-r--r--   0        0        0   115349 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmplv4pugrr.jpg
+-rw-r--r--   0        0        0    91136 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpsvh8rgjz.jpg
+-rw-r--r--   0        0        0    91363 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpvtinxpmw.jpg
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/langchain/bark_example.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/langchain/document_qa.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/langchain/example.py
+-rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/langchain/florida-drivers-license.jpeg
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/langchain/sam_example.py
+-rw-r--r--   0        0        0   209515 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/langchain/waldo.jpeg
+-rw-r--r--   0        0        0   263388 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/langchain/waldo_3.webp
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/minichain/agent.pmpt.tpl
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/minichain/agent.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/examples/minichain/example.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/__init__.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/__init__.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/bark.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/clip_interrogator.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/document_qa.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/gradio_tool.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/image_captioning.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/image_to_music.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/prompt_generator.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/sam_with_clip.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/stable_diffusion.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/text_to_video.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/gradio_tools/tools/whisper.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/scripts/format.sh
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/scripts/lint.sh
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/tests/test_sam.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/tests/test_tools.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8667 2020-02-02 00:00:00.000000 gradio_tools-0.0.8/PKG-INFO
```

### Comparing `gradio_tools-0.0.7/.DS_Store` & `gradio_tools-0.0.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/README.md` & `gradio_tools-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg` & `gradio_tools-0.0.8/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg` & `gradio_tools-0.0.8/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg` & `gradio_tools-0.0.8/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg` & `gradio_tools-0.0.8/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpd4fe9ahm.jpg` & `gradio_tools-0.0.8/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpd4fe9ahm.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpe0qa0lhx.jpg` & `gradio_tools-0.0.8/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpe0qa0lhx.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpnvmcs9su.jpg` & `gradio_tools-0.0.8/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpnvmcs9su.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpwvlf4c_7.jpg` & `gradio_tools-0.0.8/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpwvlf4c_7.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/27195f48-ea83-46b0-be72-39e76f1432a3/tmp0364mijl.jpg` & `gradio_tools-0.0.8/27195f48-ea83-46b0-be72-39e76f1432a3/tmp0364mijl.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/27195f48-ea83-46b0-be72-39e76f1432a3/tmpn8vk75sg.jpg` & `gradio_tools-0.0.8/27195f48-ea83-46b0-be72-39e76f1432a3/tmpn8vk75sg.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/27195f48-ea83-46b0-be72-39e76f1432a3/tmpp4x_v2hp.jpg` & `gradio_tools-0.0.8/27195f48-ea83-46b0-be72-39e76f1432a3/tmpp4x_v2hp.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/27195f48-ea83-46b0-be72-39e76f1432a3/tmpvswx2fg1.jpg` & `gradio_tools-0.0.8/27195f48-ea83-46b0-be72-39e76f1432a3/tmpvswx2fg1.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp37n48nis.jpg` & `gradio_tools-0.0.8/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp37n48nis.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp6_fdz6c8.jpg` & `gradio_tools-0.0.8/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp6_fdz6c8.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp_kkj0za7.jpg` & `gradio_tools-0.0.8/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp_kkj0za7.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmpbjq5o1s2.jpg` & `gradio_tools-0.0.8/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmpbjq5o1s2.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg` & `gradio_tools-0.0.8/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg` & `gradio_tools-0.0.8/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg` & `gradio_tools-0.0.8/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg` & `gradio_tools-0.0.8/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg` & `gradio_tools-0.0.8/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg` & `gradio_tools-0.0.8/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg` & `gradio_tools-0.0.8/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg` & `gradio_tools-0.0.8/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg` & `gradio_tools-0.0.8/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg` & `gradio_tools-0.0.8/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg` & `gradio_tools-0.0.8/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg` & `gradio_tools-0.0.8/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpmsy7r5s4.jpg` & `gradio_tools-0.0.8/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpmsy7r5s4.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpotr65fvw.jpg` & `gradio_tools-0.0.8/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpotr65fvw.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpr4__qxcx.jpg` & `gradio_tools-0.0.8/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpr4__qxcx.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpx4p7b1ft.jpg` & `gradio_tools-0.0.8/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpx4p7b1ft.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmpjumozfel.jpg` & `gradio_tools-0.0.8/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmpjumozfel.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmppfkjroq_.jpg` & `gradio_tools-0.0.8/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmppfkjroq_.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpj6tqr3fx.jpg` & `gradio_tools-0.0.8/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpj6tqr3fx.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpodtfruna.jpg` & `gradio_tools-0.0.8/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpodtfruna.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmppg3kuayo.jpg` & `gradio_tools-0.0.8/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmppg3kuayo.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmps600nxhc.jpg` & `gradio_tools-0.0.8/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmps600nxhc.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg` & `gradio_tools-0.0.8/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg` & `gradio_tools-0.0.8/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg` & `gradio_tools-0.0.8/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg` & `gradio_tools-0.0.8/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmp0bq293n9.jpg` & `gradio_tools-0.0.8/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmp0bq293n9.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmphhgdi5d9.jpg` & `gradio_tools-0.0.8/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmphhgdi5d9.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmpjgndeko_.jpg` & `gradio_tools-0.0.8/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmpjgndeko_.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg` & `gradio_tools-0.0.8/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg` & `gradio_tools-0.0.8/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg` & `gradio_tools-0.0.8/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg` & `gradio_tools-0.0.8/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmp74tk8cfs.jpg` & `gradio_tools-0.0.8/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmp74tk8cfs.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpk_wbbklr.jpg` & `gradio_tools-0.0.8/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpk_wbbklr.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpvufkgo26.jpg` & `gradio_tools-0.0.8/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpvufkgo26.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpz6lir7im.jpg` & `gradio_tools-0.0.8/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpz6lir7im.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpnu2s0p5c.jpg` & `gradio_tools-0.0.8/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpnu2s0p5c.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpsvafzhhw.jpg` & `gradio_tools-0.0.8/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpsvafzhhw.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpx8aicgye.jpg` & `gradio_tools-0.0.8/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpx8aicgye.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg` & `gradio_tools-0.0.8/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg` & `gradio_tools-0.0.8/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg` & `gradio_tools-0.0.8/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg` & `gradio_tools-0.0.8/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmp5myeybsm.jpg` & `gradio_tools-0.0.8/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmp5myeybsm.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpd3ufb_2o.jpg` & `gradio_tools-0.0.8/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpd3ufb_2o.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpdlfj8cj_.jpg` & `gradio_tools-0.0.8/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpdlfj8cj_.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmps0tx8a8q.jpg` & `gradio_tools-0.0.8/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmps0tx8a8q.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg` & `gradio_tools-0.0.8/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg` & `gradio_tools-0.0.8/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg` & `gradio_tools-0.0.8/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg` & `gradio_tools-0.0.8/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpg2htn2w7.jpg` & `gradio_tools-0.0.8/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpg2htn2w7.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpkoqyldk0.jpg` & `gradio_tools-0.0.8/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpkoqyldk0.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpnru9hk2q.jpg` & `gradio_tools-0.0.8/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpnru9hk2q.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpvxkwhzbo.jpg` & `gradio_tools-0.0.8/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpvxkwhzbo.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmp7n9_771q.jpg` & `gradio_tools-0.0.8/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmp7n9_771q.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpgaejg5rz.jpg` & `gradio_tools-0.0.8/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpgaejg5rz.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpl3n0u99v.jpg` & `gradio_tools-0.0.8/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpl3n0u99v.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpuylgwvrf.jpg` & `gradio_tools-0.0.8/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpuylgwvrf.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/d52f969d-6985-461d-bf02-080c86e36628/tmpe6rm8dhh.jpg` & `gradio_tools-0.0.8/d52f969d-6985-461d-bf02-080c86e36628/tmpe6rm8dhh.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/d52f969d-6985-461d-bf02-080c86e36628/tmpk6ugfnjb.jpg` & `gradio_tools-0.0.8/d52f969d-6985-461d-bf02-080c86e36628/tmpk6ugfnjb.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/d52f969d-6985-461d-bf02-080c86e36628/tmpnmfnsc82.jpg` & `gradio_tools-0.0.8/d52f969d-6985-461d-bf02-080c86e36628/tmpnmfnsc82.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/d52f969d-6985-461d-bf02-080c86e36628/tmpy8mg_mm2.jpg` & `gradio_tools-0.0.8/d52f969d-6985-461d-bf02-080c86e36628/tmpy8mg_mm2.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmphp1_2bwe.jpg` & `gradio_tools-0.0.8/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmphp1_2bwe.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmplv4pugrr.jpg` & `gradio_tools-0.0.8/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmplv4pugrr.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpsvh8rgjz.jpg` & `gradio_tools-0.0.8/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpsvh8rgjz.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpvtinxpmw.jpg` & `gradio_tools-0.0.8/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpvtinxpmw.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/examples/langchain/bark_example.py` & `gradio_tools-0.0.8/examples/langchain/bark_example.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/examples/langchain/document_qa.py` & `gradio_tools-0.0.8/examples/langchain/document_qa.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/examples/langchain/example.py` & `gradio_tools-0.0.8/examples/langchain/example.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from gradio_tools.tools import (StableDiffusionTool, ImageCaptioningTool, StableDiffusionPromptGeneratorTool,
                                 TextToVideoTool)
 
 from langchain.memory import ConversationBufferMemory
 
 llm = OpenAI(temperature=0)
 memory = ConversationBufferMemory(memory_key="chat_history")
-tools = [StableDiffusionTool().langchain, ImageCaptioningTool().langchain,
+tools = [StableDiffusionTool().langchain,
          StableDiffusionPromptGeneratorTool().langchain, TextToVideoTool().langchain]
 
 
 agent = initialize_agent(tools, llm, memory=memory, agent="conversational-react-description", verbose=True)
 output = agent.run(input=("Please create a photo of a dog riding a skateboard "
                           "but improve my prompt prior to using an image generator."
-                          "Please caption the generated image and create a video for it using the improved prompt."))
+                          "Please create a video for it using the improved prompt."))
```

### Comparing `gradio_tools-0.0.7/examples/langchain/florida-drivers-license.jpeg` & `gradio_tools-0.0.8/examples/langchain/florida-drivers-license.jpeg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/examples/langchain/sam_example.py` & `gradio_tools-0.0.8/examples/langchain/sam_example.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 
 
 
 agent = initialize_agent(tools, llm, memory=memory, agent="conversational-react-description", verbose=True)
 output = agent.run(input=(f"Please find Waldo in this image: {waldo_1}. "
                           "Waldo is a man with glasses wearing sweater with red and white stripes"))
 print(output)
-output = agent.run(input=(f"Great job! Now find Waldo in this image: {waldo_2}."))
+output = agent.run(input=(f"Great job! Now find Waldo in this image: {waldo_2}. "
+                          "Set the clip_threshold to 0.9"))
 print(output)
```

### Comparing `gradio_tools-0.0.7/examples/langchain/waldo.jpeg` & `gradio_tools-0.0.8/examples/langchain/waldo.jpeg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/examples/langchain/waldo_3.webp` & `gradio_tools-0.0.8/examples/langchain/waldo_3.webp`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/examples/minichain/agent.pmpt.tpl` & `gradio_tools-0.0.8/examples/minichain/agent.pmpt.tpl`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/examples/minichain/agent.py` & `gradio_tools-0.0.8/examples/minichain/agent.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/examples/minichain/example.py` & `gradio_tools-0.0.8/examples/minichain/example.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/gradio_tools/__init__.py` & `gradio_tools-0.0.8/gradio_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from gradio_tools.tools import (BarkTextToSpeechTool, ClipInterrogatorTool,
                                 DocQueryDocumentAnsweringTool, GradioTool,
                                 ImageCaptioningTool, ImageToMusicTool,
+                                SAMImageSegmentationTool,
                                 StableDiffusionPromptGeneratorTool,
                                 StableDiffusionTool, TextToVideoTool,
-                                WhisperAudioTranscriptionTool,
-                                SAMImageSegmentationTool)
+                                WhisperAudioTranscriptionTool)
 
 __all__ = [
     "GradioTool",
     "StableDiffusionTool",
     "ClipInterrogatorTool",
     "ImageCaptioningTool",
     "ImageToMusicTool",
     "WhisperAudioTranscriptionTool",
     "StableDiffusionPromptGeneratorTool",
     "TextToVideoTool",
     "DocQueryDocumentAnsweringTool",
     "BarkTextToSpeechTool",
-    "SAMImageSegmentationTool"
+    "SAMImageSegmentationTool",
 ]
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/__init__.py` & `gradio_tools-0.0.8/gradio_tools/tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from gradio_tools.tools.clip_interrogator import ClipInterrogatorTool
 from gradio_tools.tools.document_qa import DocQueryDocumentAnsweringTool
 from gradio_tools.tools.gradio_tool import GradioTool
 from gradio_tools.tools.image_captioning import ImageCaptioningTool
 from gradio_tools.tools.image_to_music import ImageToMusicTool
 from gradio_tools.tools.prompt_generator import \
     StableDiffusionPromptGeneratorTool
+from gradio_tools.tools.sam_with_clip import SAMImageSegmentationTool
 from gradio_tools.tools.stable_diffusion import StableDiffusionTool
 from gradio_tools.tools.text_to_video import TextToVideoTool
 from gradio_tools.tools.whisper import WhisperAudioTranscriptionTool
-from gradio_tools.tools.sam_with_clip import SAMImageSegmentationTool
 
 __all__ = [
     "GradioTool",
     "StableDiffusionTool",
     "ClipInterrogatorTool",
     "ImageCaptioningTool",
     "ImageToMusicTool",
     "WhisperAudioTranscriptionTool",
     "StableDiffusionPromptGeneratorTool",
     "TextToVideoTool",
     "DocQueryDocumentAnsweringTool",
     "BarkTextToSpeechTool",
-    "SAMImageSegmentationTool"
+    "SAMImageSegmentationTool",
 ]
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/bark.py` & `gradio_tools-0.0.8/gradio_tools/tools/bark.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from gradio_client.client import Job
 
 from gradio_tools.tools.gradio_tool import GradioTool
 
 if TYPE_CHECKING:
     import gradio as gr
@@ -76,12 +76,12 @@
         else:
             speaker = "Unconditional"
         return self.client.submit(text, speaker, fn_index=3)
 
     def postprocess(self, output: str) -> str:
         return output
 
-    def _block_input(self, gr) -> "gr.components.Component":
-        return gr.Textbox()
+    def _block_input(self, gr) -> List["gr.components.Component"]:
+        return [gr.Textbox()]
 
-    def _block_output(self, gr) -> "gr.components.Component":
-        return gr.Audio()
+    def _block_output(self, gr) -> List["gr.components.Component"]:
+        return [gr.Audio()]
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/clip_interrogator.py` & `gradio_tools-0.0.8/gradio_tools/tools/clip_interrogator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from gradio_client.client import Job
 
 from gradio_tools.tools.gradio_tool import GradioTool
 
 if TYPE_CHECKING:
     import gradio as gr
@@ -27,9 +27,9 @@
         return self.client.submit(
             query, "ViT-L (best for Stable Diffusion 1.*)", "best", fn_index=3
         )
 
     def postprocess(self, output: str) -> str:
         return output
 
-    def _block_input(self, gr) -> "gr.components.Component":
-        return gr.Image()
+    def _block_input(self, gr) -> List["gr.components.Component"]:
+        return [gr.Image()]
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/document_qa.py` & `gradio_tools-0.0.8/gradio_tools/tools/document_qa.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from gradio_client.client import Job
 
 from gradio_tools.tools.gradio_tool import GradioTool
 
 if TYPE_CHECKING:
     import gradio as gr
 
 
 class DocQueryDocumentAnsweringTool(GradioTool):
     def __init__(
         self,
         name="DocQuery",
         description=(
-            "A tool for answering questions about a document from the from the image of the document. Input will be a two strings separated by a comma: the first will be the path or URL to an image of a document. The second will be your question about the document."
+            "A tool for answering questions about a document from the from the image of the document. Input will be a two strings separated by a |: the first will be the path or URL to an image of a document. The second will be your question about the document."
             "The output will the text answer to your question."
         ),
         src="abidlabs/docquery",
         hf_token=None,
         duplicate=True,
     ) -> None:
         super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
-        img, question = query.split(",")
+        img, question = query.split("|")
         return self.client.submit(img.strip(), question.strip(), api_name="/predict")
 
     def postprocess(self, output: str) -> str:
         return output
 
-    def _block_input(self, gr) -> "gr.components.Component":
-        return gr.Image()
+    def _block_input(self, gr) -> List["gr.components.Component"]:
+        return [gr.Image(), gr.Textbox()]
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/gradio_tool.py` & `gradio_tools-0.0.8/gradio_tools/tools/gradio_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import time
 from abc import abstractmethod
-from typing import Any, Tuple, Union
+from typing import Any, List, Tuple, Union
 
 import gradio_client as grc
 import huggingface_hub
 from gradio_client.client import Job
 from gradio_client.utils import QueueError
 
 try:
@@ -66,33 +66,33 @@
         try:
             output = self.postprocess(job.result())
         except QueueError:
             output = "QUEUE_FULL"
         return output
 
     # Optional gradio functionalities
-    def _block_input(self, gr) -> "gr.components.Component":
-        return gr.Textbox()
+    def _block_input(self, gr) -> List["gr.components.Component"]:
+        return [gr.Textbox()]
 
-    def _block_output(self, gr) -> "gr.components.Component":
-        return gr.Textbox()
+    def _block_output(self, gr) -> List["gr.components.Component"]:
+        return [gr.Textbox()]
 
-    def block_input(self) -> "gr.components.Component":
+    def block_input(self) -> List["gr.components.Component"]:
         try:
             import gradio as gr
 
             GRADIO_INSTALLED = True
         except (ModuleNotFoundError, ImportError):
             GRADIO_INSTALLED = False
         if not GRADIO_INSTALLED:
             raise ModuleNotFoundError("gradio must be installed to call block_input")
         else:
             return self._block_input(gr)
 
-    def block_output(self) -> "gr.components.Component":
+    def block_output(self) -> List["gr.components.Component"]:
         try:
             import gradio as gr
 
             GRADIO_INSTALLED = True
         except (ModuleNotFoundError, ImportError):
             GRADIO_INSTALLED = False
         if not GRADIO_INSTALLED:
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/image_captioning.py` & `gradio_tools-0.0.8/gradio_tools/tools/image_captioning.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from gradio_client.client import Job
 
 from gradio_tools.tools.gradio_tool import GradioTool
 
 if TYPE_CHECKING:
     import gradio as gr
@@ -17,24 +17,24 @@
         self,
         name="ImageCaptioner",
         description=(
             "An image captioner. Use this to create a caption for an image. "
             "Input will be a path to an image file. "
             "The output will be a caption of that image."
         ),
-        src="taesiri/BLIP-2",
+        src="gradio-client-demos/BLIP-2",
         hf_token=None,
         duplicate=True,
     ) -> None:
         super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
         return self.client.submit(query.strip("'"), "Beam Search", fn_index=0)
 
     def postprocess(self, output: str) -> str:
         return output  # type: ignore
 
-    def _block_input(self, gr) -> "gr.components.Component":
-        return gr.Image()
+    def _block_input(self, gr) -> List["gr.components.Component"]:
+        return [gr.Image()]
 
-    def _block_output(self, gr) -> "gr.components.Component":
-        return gr.Textbox()
+    def _block_output(self, gr) -> List["gr.components.Component"]:
+        return [gr.Textbox()]
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/image_to_music.py` & `gradio_tools-0.0.8/gradio_tools/tools/stable_diffusion.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,46 @@
-from typing import TYPE_CHECKING, Any, Tuple, Union
+from __future__ import annotations
+
+import os
+from typing import TYPE_CHECKING, Any, List, Tuple
 
 from gradio_client.client import Job
 
 from gradio_tools.tools.gradio_tool import GradioTool
 
 if TYPE_CHECKING:
     import gradio as gr
 
 
-class ImageToMusicTool(GradioTool):
+class StableDiffusionTool(GradioTool):
+    """Tool for calling stable diffusion from llm"""
+
     def __init__(
         self,
-        name="ImagetoMusic",
+        name="StableDiffusion",
         description=(
-            "A tool for creating music from images. Use this tool to create a musical "
-            "track from an image. Input will be a path to an image file. "
-            "The output will be an audio file generated from that image."
+            "An image generator. Use this to generate images based on "
+            "text input. Input should be a description of what the image should "
+            "look like. The output will be a path to an image file."
         ),
-        src="fffiloni/img-to-music",
+        src="gradio-client-demos/stable-diffusion",
         hf_token=None,
         duplicate=False,
     ) -> None:
         super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
-        return self.client.submit(
-            query.strip("'"), 15, "medium", "loop", None, fn_index=0
-        )
+        return self.client.submit(query, "", 9, fn_index=1)
 
-    def postprocess(self, output: Union[Tuple[Any], Any]) -> str:
-        return output[1]  # type: ignore
+    def postprocess(self, output: Tuple[Any] | Any) -> str:
+        assert isinstance(output, str)
+        return [
+            os.path.join(output, i)
+            for i in os.listdir(output)
+            if not i.endswith("json")
+        ][0]
 
-    def _block_input(self, gr) -> "gr.components.Component":
-        return gr.Image()
+    def _block_input(self, gr) -> List["gr.components.Component"]:
+        return [gr.Textbox()]
 
-    def _block_output(self, gr) -> "gr.components.Component":
-        return gr.Audio()
+    def _block_output(self, gr) -> List["gr.components.Component"]:
+        return [gr.Image()]
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/prompt_generator.py` & `gradio_tools-0.0.8/gradio_tools/tools/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/sam_with_clip.py` & `gradio_tools-0.0.8/gradio_tools/tools/sam_with_clip.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from gradio_client.client import Job
 
 from gradio_tools.tools.gradio_tool import GradioTool
 
 if TYPE_CHECKING:
     import gradio as gr
 
 
-
 class SAMImageSegmentationTool(GradioTool):
     """Tool for segmenting images based on natural language queries."""
 
     def __init__(
         self,
         name="SAMImageSegmentation",
         description=(
@@ -32,24 +31,36 @@
         hf_token=None,
         duplicate=False,
     ) -> None:
         super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
         try:
-            image, query, predicted_iou_threshold, stability_score_threshold, clip_threshold = query.split("|")
+            (
+                image,
+                query,
+                predicted_iou_threshold,
+                stability_score_threshold,
+                clip_threshold,
+            ) = query.split("|")
         except ValueError as e:
-            raise ValueError("Not enough arguments passed to the SAMImageSegmentationTool! " 
-                             "Expected 5 (image, query, predicted_iou_threshold, stability_score_threshold, clip_threshold)") from e
-        return self.client.submit(float(predicted_iou_threshold),
-                                  float(stability_score_threshold),
-                                  float(clip_threshold),
-                                  image, query.strip(), api_name="/predict")
+            raise ValueError(
+                "Not enough arguments passed to the SAMImageSegmentationTool! "
+                "Expected 5 (image, query, predicted_iou_threshold, stability_score_threshold, clip_threshold)"
+            ) from e
+        return self.client.submit(
+            float(predicted_iou_threshold),
+            float(stability_score_threshold),
+            float(clip_threshold),
+            image,
+            query.strip(),
+            api_name="/predict",
+        )
 
     def postprocess(self, output: str) -> str:
         return output
 
-    def _block_input(self, gr) -> "gr.components.Component":
-        return gr.Textbox()
+    def _block_input(self, gr) -> List["gr.components.Component"]:
+        return [gr.Number(), gr.Number(), gr.Number(), gr.Image(), gr.Textbox()]
 
-    def _block_output(self, gr) -> "gr.components.Component":
-        return gr.Audio()
+    def _block_output(self, gr) -> List["gr.components.Component"]:
+        return [gr.Image()]
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/text_to_video.py` & `gradio_tools-0.0.8/gradio_tools/tools/text_to_video.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from gradio_client.client import Job
 
 from gradio_tools.tools.gradio_tool import GradioTool
 
 if TYPE_CHECKING:
     import gradio as gr
@@ -26,9 +26,9 @@
 
     def create_job(self, query: str) -> Job:
         return self.client.submit(query, -1, 16, 25, fn_index=1)
 
     def postprocess(self, output: str) -> str:
         return output
 
-    def _block_output(self, gr) -> "gr.components.Component":
-        return gr.Video()
+    def _block_output(self, gr) -> List["gr.components.Component"]:
+        return [gr.Video()]
```

### Comparing `gradio_tools-0.0.7/gradio_tools/tools/whisper.py` & `gradio_tools-0.0.8/gradio_tools/tools/whisper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from gradio_client.client import Job
 
 from gradio_tools.tools.gradio_tool import GradioTool
 
 if TYPE_CHECKING:
     import gradio as gr
@@ -27,9 +27,9 @@
 
     def create_job(self, query: str) -> Job:
         return self.client.submit(query, api_name="/predict")
 
     def postprocess(self, output: str) -> str:
         return output
 
-    def _block_input(self, gr) -> "gr.components.Component":
-        return gr.Audio()
+    def _block_input(self, gr) -> List["gr.components.Component"]:
+        return [gr.Audio()]
```

### Comparing `gradio_tools-0.0.7/tests/test_sam.py` & `gradio_tools-0.0.8/tests/test_sam.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/LICENSE` & `gradio_tools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.7/pyproject.toml` & `gradio_tools-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt", "hatch-fancy-pypi-readme>=22.5.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_tools"
-version = "0.0.7"
+version = "0.0.8"
 description = "Use Gradio Apps as tools for LLM Agents"
 requires-python = ">=3.8"
 license = "MIT"
 authors = [
     { name = "Freddy Boulton", email = "alfonsoboulton@gmail.com" },
 ]
 classifiers = [
```

### Comparing `gradio_tools-0.0.7/PKG-INFO` & `gradio_tools-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Use Gradio Apps as tools for LLM Agents
 Author-email: Freddy Boulton <alfonsoboulton@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

