This site contains public domain implementations of FIDO Device Onboard.

FIDO Device Onboard (FDO) is a protocol that allows a _Device_ to automatically onboard to a server (the _Owner_), so that the Device is henceforth controlled by this server.  An intermediate _Rendezvous Server_ is used to help the Device find the Owner.

FDO originated at [Intel Corporation](https://www.intel.com) (originally under the name of "Secure Device Onboard" (SDO)) and was donated by Intel to the FIDO Alliance for standardization as FDO.  The FIDO Alliance maintains the specifications for FDO, currently at version 1.1 ([FDO Specification](https://fidoalliance.org/specifications/download-iot-specifications/)).

As of 2025-05-05, there are three supported implementations of FDO served in this site:

* A [Java-based implementation](https://github.com/secure-device-onboard/pri-fidoiot) of FDO client, server and rendezvous server
* A GO-based implementation of FDO [client](https://github.com/fido-device-onboard/go-fdo-client), [server & rendezvous server](https://github.com/fido-device-onboard/go-fdo-server)
* A [C-based implementation](https://github.com/secure-device-onboard/client-sdk-fidoiot) of the FDO client only

We are also familiar with a Rust-based implementation of FDO, stored in [another site](https://github.com/fdo-rs/fido-device-onboard-rs).  Please query for support and other information there.

Support for the original Secure Device Onboard (SDO) was discontinued on March 31, 2023.

# Repositories

Secure Device Onboard organization implementations for both FIDO Device Onboard (FDO) specification
as well as Secure Device Onboard (SDO) protocol.

## FDO Specific Repositories

The following repositories are created to support implementations for FDO specification.

| Repository&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Description |
|---|---|
| [client-sdk-fidoiot](https://github.com/secure-device-onboard/client-sdk-fidoiot) | C-based reference implementation for Device component defined in FDO specification. |
| [pri-fidoiot](https://github.com/secure-device-onboard/pri-fidoiot) | JAVA-based reference implementation for all components defined in FDO specification. |
| [release-fidoiot](https://github.com/secure-device-onboard/release-fidoiot) | Hosts binary artifacts of different tagged releases of FDO specification implementations. |
| [test-fidoiot](https://github.com/secure-device-onboard/test-fidoiot) | TestNG-based test code used to validate pull requests in pri-fidoiot and client-sdk-fidoiot repositories. |

## SDO Specific Repositories (legacy)

The following repositories are created to support implementations for SDO protocol.

| Repository&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Description |
|---|---|
| [all-in-one-demo](https://github.com/secure-device-onboard/all-in-one-demo) | JAVA and Docker based solution to host all service components (Owner, Manufacturer, Rendezvous) defined in SDO protocol. Reuses binaries from iot-platform-sdk, pri, supply-chain-tools and rendezvous-service. |
| [client-sdk](https://github.com/secure-device-onboard/client-sdk) | C-based reference implementation for Device component defined in SDO protocol. |
| [iot-platform-sdk](https://github.com/secure-device-onboard/iot-platform-sdk) | JAVA-based reference implementation for Owner component defined in SDO protocol. |
| [pri](https://github.com/secure-device-onboard/pri) | JAVA-based reference implementation for all components defined in SDO protocol. |
| [rendezvous-service](https://github.com/secure-device-onboard/rendezvous-service) | JAVA-based reference implementation for Rendezvous component defined in SDO protocol. |
| [release](https://github.com/secure-device-onboard/release-fidoiot) | Hosts binary artifacts of different tagged releases of FDO protocol implementations. |
| [supply-chain-tools](https://github.com/secure-device-onboard/supply-chain-tools) | JAVA-based reference implementation for Manufacturer and Reseller component defined in SDO protocol. |

## Common repositories

The following repositories contain artifacts related to both FDO as well as SDO releases.

| Repository&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Description |
|---|---|
| [docs](https://github.com/secure-device-onboard/docs) | Maintains source for the documents hosted on [GitHub IO](https://secure-device-onboard.github.io/docs). |
| [epid-verification-service](https://github.com/secure-device-onboard/epid-verification-service) | JAVA-based implementation to support EPID signature verification through REST end-points. |
| [readme](https://github.com/secure-device-onboard/readme) | Contains details about different repositories within Secure Device Onboard organization. |
