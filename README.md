# How to use

This repo builds `libdxcompiler.{dylib,so,dll}` from
[Traverse-Research/DirectXShaderCompiler][fork] (our fork of microsoft/DirectXShaderCompiler) so we can ship our patches — currently the
SPIR-V `-fspv-allow-import` flag for Import linkage in `lib_*` targets.

1. Check out the repo
2. Update [`commit-hash`](./commit-hash) to point to the desired commit on
   the fork's `main` (or any branch HEAD if you're testing a topic branch)
3. Download the build artifacts from the workflow run
4. Unzip all artifacts into the right directories in `breda` (`crates/breda-shader-compiler/dxc/<triple>/`)
5. When on macOS, issue `xattr -d com.apple.quarantine libdxcompiler.dylib` to de-quarantine the library (your browser will quarantine executable files, we'll need to tell macOS)

[fork]: https://github.com/Traverse-Research/DirectXShaderCompiler
