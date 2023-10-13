npm WARN deprecated safe-event-emitter@1.0.1: Renamed to @metamask/safe-event-emitter
npm WARN deprecated readdir-scoped-modules@1.1.0: This functionality has been moved to @npmcli/fs
npm WARN deprecated @npmcli/move-file@1.1.2: This functionality has been moved to @npmcli/fs
npm WARN deprecated mkdirp-promise@5.0.1: This package is broken and no longer maintained. 'mkdirp' itself supports promises now, please switch to that.
npm WARN deprecated multiaddr-to-uri@8.0.0: This module is deprecated, please upgrade to @multiformats/multiaddr-to-uri
npm WARN deprecated read-package-tree@5.3.1: The functionality that this package provided is now in @npmcli/arborist
npm WARN deprecated har-validator@5.1.5: this library is no longer supported
npm WARN deprecated eth-sig-util@1.4.2: Deprecated in favor of '@metamask/eth-sig-util'
npm WARN deprecated cids@1.1.9: This module has been superseded by the multiformats module
npm WARN deprecated cids@1.1.9: This module has been superseded by the multiformats module
npm WARN deprecated ethereumjs-block@2.2.2: New package name format for new versions: @ethereumjs/block. Please update.
npm WARN deprecated ethereumjs-tx@2.1.2: New package name format for new versions: @ethereumjs/tx. Please update.
npm WARN deprecated eth-json-rpc-errors@1.1.1: Package renamed: https://www.npmjs.com/package/eth-rpc-errors
npm WARN deprecated multicodec@1.0.4: This module has been superseded by the multiformats module
npm WARN deprecated uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated eth-json-rpc-errors@2.0.2: Package renamed: https://www.npmjs.com/package/eth-rpc-errors
npm WARN deprecated multibase@4.0.6: This module has been superseded by the multiformats module
npm WARN deprecated multibase@4.0.6: This module has been superseded by the multiformats module
npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
npm WARN deprecated ethereumjs-tx@1.3.7: New package name format for new versions: @ethereumjs/tx. Please update.
npm WARN deprecated multibase@0.6.1: This module has been superseded by the multiformats module
npm WARN deprecated multibase@0.7.0: This module has been superseded by the multiformats module
npm WARN deprecated multiaddr@10.0.1: This module is deprecated, please upgrade to @multiformats/multiaddr
npm WARN deprecated multiaddr@9.0.2: This module is deprecated, please upgrade to @multiformats/multiaddr
npm WARN deprecated multicodec@0.5.7: This module has been superseded by the multiformats module
npm WARN deprecated multicodec@3.2.1: This module has been superseded by the multiformats module
npm WARN deprecated multicodec@3.2.1: This module has been superseded by the multiformats module
npm WARN deprecated ethereumjs-vm@2.6.0: New package name format for new versions: @ethereumjs/vm. Please update.
npm WARN deprecated ethereumjs-block@1.7.1: New package name format for new versions: @ethereumjs/block. Please update.
npm WARN deprecated ethereumjs-common@1.5.2: New package name format for new versions: @ethereumjs/common. Please update.
npm WARN deprecated libp2p-noise@2.0.5: This repository is now being maintained by ChainSafe, and can be found at https://github.com/ChainSafe/js-libp2p-noise under @chainsafe/libp2p-noise
npm WARN deprecated cids@0.7.5: This module has been superseded by the multiformats module
npm WARN cleanup Failed to remove some directories [
npm WARN cleanup   [
npm WARN cleanup     '/workspace/dto-validator/node_modules/libp2p-mdns/node_modules/ursa-optional',
npm WARN cleanup     [Error: ENOTEMPTY: directory not empty, rmdir '/workspace/dto-validator/node_modules/libp2p-mdns/node_modules/ursa-optional'] {
npm WARN cleanup       errno: -39,
npm WARN cleanup       code: 'ENOTEMPTY',
npm WARN cleanup       syscall: 'rmdir',
npm WARN cleanup       path: '/workspace/dto-validator/node_modules/libp2p-mdns/node_modules/ursa-optional'
npm WARN cleanup     }
npm WARN cleanup   ],
npm WARN cleanup   [
npm WARN cleanup     '/workspace/dto-validator/node_modules/libp2p-noise/node_modules/ursa-optional',
npm WARN cleanup     [Error: ENOTEMPTY: directory not empty, rmdir '/workspace/dto-validator/node_modules/libp2p-noise/node_modules/ursa-optional'] {
npm WARN cleanup       errno: -39,
npm WARN cleanup       code: 'ENOTEMPTY',
npm WARN cleanup       syscall: 'rmdir',
npm WARN cleanup       path: '/workspace/dto-validator/node_modules/libp2p-noise/node_modules/ursa-optional'
npm WARN cleanup     }
npm WARN cleanup   ]
npm WARN cleanup ]
npm ERR! code 1
npm ERR! path /workspace/dto-validator/node_modules/bcrypto
npm ERR! command failed
npm ERR! command sh -c node-gyp rebuild
npm ERR! gyp info it worked if it ends with ok
npm ERR! gyp info using node-gyp@5.1.1
npm ERR! gyp info using node@18.15.0 | linux | x64
npm ERR! gyp info find Python using Python version 3.11.1 found at "/home/gitpod/.pyenv/versions/3.11.1/bin/python"
npm ERR! (node:1401) [DEP0150] DeprecationWarning: Setting process.config is deprecated. In the future the property will be read-only.
npm ERR! (Use `node --trace-deprecation ...` to show where the warning was created)
npm ERR! gyp info spawn /home/gitpod/.pyenv/versions/3.11.1/bin/python
npm ERR! gyp info spawn args [
npm ERR! gyp info spawn args   '/workspace/dto-validator/node_modules/node-gyp/gyp/gyp_main.py',
npm ERR! gyp info spawn args   'binding.gyp',
npm ERR! gyp info spawn args   '-f',
npm ERR! gyp info spawn args   'make',
npm ERR! gyp info spawn args   '-I',
npm ERR! gyp info spawn args   '/workspace/dto-validator/node_modules/bcrypto/build/config.gypi',
npm ERR! gyp info spawn args   '-I',
npm ERR! gyp info spawn args   '/workspace/dto-validator/node_modules/node-gyp/addon.gypi',
npm ERR! gyp info spawn args   '-I',
npm ERR! gyp info spawn args   '/home/gitpod/.cache/node-gyp/18.15.0/include/node/common.gypi',
npm ERR! gyp info spawn args   '-Dlibrary=shared_library',
npm ERR! gyp info spawn args   '-Dvisibility=default',
npm ERR! gyp info spawn args   '-Dnode_root_dir=/home/gitpod/.cache/node-gyp/18.15.0',
npm ERR! gyp info spawn args   '-Dnode_gyp_dir=/workspace/dto-validator/node_modules/node-gyp',
npm ERR! gyp info spawn args   '-Dnode_lib_file=/home/gitpod/.cache/node-gyp/18.15.0/<(target_arch)/node.lib',
npm ERR! gyp info spawn args   '-Dmodule_root_dir=/workspace/dto-validator/node_modules/bcrypto',
npm ERR! gyp info spawn args   '-Dnode_engine=v8',
npm ERR! gyp info spawn args   '--depth=.',
npm ERR! gyp info spawn args   '--no-parallel',
npm ERR! gyp info spawn args   '--generator-output',
npm ERR! gyp info spawn args   'build',
npm ERR! gyp info spawn args   '-Goutput_dir=.'
npm ERR! gyp info spawn args ]
npm ERR! Traceback (most recent call last):
npm ERR!   File "/workspace/dto-validator/node_modules/node-gyp/gyp/gyp_main.py", line 50, in <module>
npm ERR!     sys.exit(gyp.script_main())
npm ERR!              ^^^^^^^^^^^^^^^^^
npm ERR!   File "/workspace/dto-validator/node_modules/node-gyp/gyp/pylib/gyp/__init__.py", line 554, in script_main
npm ERR!     return main(sys.argv[1:])
npm ERR!            ^^^^^^^^^^^^^^^^^^
npm ERR!   File "/workspace/dto-validator/node_modules/node-gyp/gyp/pylib/gyp/__init__.py", line 547, in main
npm ERR!     return gyp_main(args)
npm ERR!            ^^^^^^^^^^^^^^
npm ERR!   File "/workspace/dto-validator/node_modules/node-gyp/gyp/pylib/gyp/__init__.py", line 520, in gyp_main
npm ERR!     [generator, flat_list, targets, data] = Load(
npm ERR!                                             ^^^^^
npm ERR!   File "/workspace/dto-validator/node_modules/node-gyp/gyp/pylib/gyp/__init__.py", line 136, in Load
npm ERR!     result = gyp.input.Load(build_files, default_variables, includes[:],
npm ERR!              ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
npm ERR!   File "/workspace/dto-validator/node_modules/node-gyp/gyp/pylib/gyp/input.py", line 2782, in Load
npm ERR!     LoadTargetBuildFile(build_file, data, aux_data,
npm ERR!   File "/workspace/dto-validator/node_modules/node-gyp/gyp/pylib/gyp/input.py", line 391, in LoadTargetBuildFile
npm ERR!     build_file_data = LoadOneBuildFile(build_file_path, data, aux_data,
npm ERR!                       ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
npm ERR!   File "/workspace/dto-validator/node_modules/node-gyp/gyp/pylib/gyp/input.py", line 234, in LoadOneBuildFile
npm ERR!     build_file_contents = open(build_file_path, 'rU').read()
npm ERR!                           ^^^^^^^^^^^^^^^^^^^^^^^^^^^
npm ERR! ValueError: invalid mode: 'rU' while trying to load binding.gyp
npm ERR! gyp ERR! configure error 
npm ERR! gyp ERR! stack Error: `gyp` failed with exit code: 1
npm ERR! gyp ERR! stack     at ChildProcess.onCpExit (/workspace/dto-validator/node_modules/node-gyp/lib/configure.js:351:16)
npm ERR! gyp ERR! stack     at ChildProcess.emit (node:events:513:28)
npm ERR! gyp ERR! stack     at ChildProcess._handle.onexit (node:internal/child_process:291:12)
npm ERR! gyp ERR! System Linux 5.15.0-47-generic
npm ERR! gyp ERR! command "/home/gitpod/.nvm/versions/node/v18.15.0/bin/node" "/workspace/dto-validator/node_modules/.bin/node-gyp" "rebuild"
npm ERR! gyp ERR! cwd /workspace/dto-validator/node_modules/bcrypto
npm ERR! gyp ERR! node -v v18.15.0
npm ERR! gyp ERR! node-gyp -v v5.1.1
npm ERR! gyp ERR! not ok

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/gitpod/.npm/_logs/2023-04-17T14_49_24_826Z-debug-0.log
