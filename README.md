# flutter_rust_example

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Rust

// prerequisite
installing visual studio option desktop C

// Create library
cargo new rust --vcs=none --lib

cargo install flutter_rust_bridge_codegen

dart pub global activate ffigen

lutter pub add flutter_rust_bridge

flutter pub add -d build_runner

flutter pub add -d freezed

flutter pub add freezed_annotation

cargo install cargo-ndk

flutter pub add --dev ffigen && flutter pub add ffi

flutter_rust_bridge_codegen --rust-input rust/src/api.rs --dart-output lib/bridge_generated.dart
