These libraries are required for some Indy components to work correctly in this project.

They provide the OpenSSL runtime files needed by components that use TLS/SSL, certificate handling, and secure network connections. Without them, features depending on Indy and OpenSSL may fail at runtime or not initialize properly.

These binaries were downloaded from https://github.com/IndySockets/OpenSSL-Binaries and are kept in this folder as part of the project dependencies. The current version in use is # openssl-1.0.2u.

They should be updated from time to time to keep the build aligned with the latest supported OpenSSL versions and security fixes.

In the project, a post-build event is configured so that the DLL files are automatically copied to the compilation output folder. This ensures the generated executable can find the required libraries when it runs without manual intervention.
