# Distributed Social Identity (DSI)

This repository contains the draft specification for **Distributed Social Identity (DSI)**, a decentralized profile format based on vCard 4.0. The specification introduces extensions to support distributed social networks, enabling users to maintain control over their identity while ensuring interoperability with decentralized ecosystems.

## Purpose

The DSI specification aims to provide a standardized and extensible format for representing decentralized social identities. By leveraging the vCard 4.0 format and introducing custom properties, the specification allows users to:

- Define canonical sources for their vCard profiles using the `SOURCE` property.
- Associate RSS/Atom feeds with their profiles using the `X-FEED` property.
- Include social media identifiers and endorsements in a structured, machine-readable format.
- Support cryptographic identity verification through public keys and signatures.
- Enable key rotation and revocation for enhanced security.

## Key Features

- **Decentralized Identity**: Users can self-host their vCard profiles, ensuring full control over their identity.
- **Feed Integration**: Profiles can include RSS/Atom feeds to provide updates, posts, or activity streams.
- **Extensibility**: Custom properties (e.g., `X-FEED`, `X-ENDORSE`, `X-<PLATFORM>`) allow for future extensions without breaking compatibility.
- **Security**: Supports Ed25519 cryptographic keys for signing and verifying identity-related data.
- **Interoperability**: Ensures compatibility with existing vCard systems while enabling decentralized use cases.

## Structure

The draft specification is located in the `draft/` directory:

- **`draft-desvelao-dsi-00.rfc`**: The main document defining the DSI specification.

## Example Use Case

A user can create a vCard profile with the following properties:

- A canonical `SOURCE` URL pointing to the vCard file.
- Public keys for identity verification.
- RSS feeds for sharing updates.
- Endorsements from other identities in the network.

## Status

This document is an **Internet-Draft** and is not an Internet Standards Track specification. It is published for informational purposes and may be used freely for software implementation, federation protocols, or identity systems.

## License

This repository is open for public use under the terms specified in the draft document.

## Contributing

Contributions to the draft are welcome. Please submit issues or pull requests to suggest improvements or report errors.