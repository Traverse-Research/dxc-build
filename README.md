# How to use

1. Check out the repo
2. Update [`commit-hash`](./commit-hash) to point to the right dxc commit hash
3. Download the build artifacts
4. Unzip all artifacts into the right directories in `breda` (`crates/breda-shader-compiler/dxc/<triple>/`)
5. When on macOS, issue `xattr -d com.apple.quarantine libdxcompiler.dylib` to de-quarantine the library (your browser will quarantine executable files, we'll need to tell macOS)
