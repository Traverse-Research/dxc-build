# How to use

1. Check out the repo
2. Update `commit-hash` to point to the right dxc commit hash
3. Download the build artifact
4. Unzip and run `xattr -d com.apple.quarantine libdxcompiler.dylib` to de-quarantine the library (your browser will quarantine executable files, we'll need to tell macOS)
5. Place file in the correct directory in breda.