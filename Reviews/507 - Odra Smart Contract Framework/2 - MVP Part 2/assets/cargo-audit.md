```
Fetching advisory database from `https://github.com/RustSec/advisory-db.git`
    Loaded 456 security advisories (from /.cargo/advisory-db)
Updating crates.io index
Scanning Cargo.lock for vulnerabilities (93 crate dependencies)
Crate:     cpufeatures
Version:   0.2.4
Warning:   yanked
Dependency tree:
cpufeatures 0.2.4
└── sha2 0.9.9
    └── ed25519-dalek 1.0.1
        └── casper-types 1.5.0
            └── odra-types 0.1.0
                ├── odra-utils 0.1.0
                │   ├── odra-mock-vm 0.1.0
                │   │   └── odra 0.1.0
                │   │       └── odra-proc-macros 0.1.0
                │   │           └── odra 0.1.0
                │   ├── odra-codegen 0.1.0
                │   │   └── odra-proc-macros 0.1.0
                │   └── odra 0.1.0
                ├── odra-test-env-wrapper 0.1.0
                │   └── odra 0.1.0
                ├── odra-mock-vm 0.1.0
                └── odra 0.1.0

warning: 1 allowed warning found
```