# Welcome, Good people!

<table>
  <tr>
    <td><img src="readme/amuletz.svg#play" style="width: 280px;"></td>
    <td><img src="readme/logo.svg" style="width: 600px;"></td>
  </tr>
</table>

## Introduction

This repository serves as a hub for the DeCent-Core project. 

The current release state is: ***usable prototype***

DeCent-Core allows users to use DWAs to access Web420.

The application is written in Kotlin and uses Kotlin Multiplatform to target Windows, Linux, Android, and MacOS. The codebase will be open-sourced shortly, more below.

## Overview 

DeCent-Core is an easy-to-use implementation of the DCNT server protocol. DeCent-Core provides two key functionalities:

- A simple interface for managing a self-hosted DCNT instance.
- A simple interface for installing and hosting decentralized web applications (DWAs) locally.

Self-hosting a DCNT server instance allows a user's web apps to receive proxied requests from within their networks, through a WebSocket connection to the locally-running DCNT server.

This allows specially designed web applications (DWAs) to use the available local connection to the DCNT server to receive connection requests and create WebRTC peer-to-peer connections directly to another web application, enabling an entirely new class of never-before possible web applications to exist: DWAs.

In addition to facilitating connections between DWAs, DeCent-Core also offers the option of hosting installable (from ZIP archive) web apps and hosting them locally for the user. This allows users to select specific, trusted web applications, store the HTML/CSS/JS files locally, and then host the executing app code for the user in an SSL/TLS context. The SSL/TLS context allows the locally running web app to create WebRTC connections to other users, which will be signaled as described above.

By using DeCent-Core in conjunction with a trusted DWA, users are able to attain complete privacy through total control.

## System Requirements

In order to use DeCent-Core, you will need:

- A device running a compatible OS
- Network access (public or private)
- A modern web browser (Firefox is highly recommended)
- (***Optional***) VPN or tunneling service
- (***Optional***) (*Coming soon*) Domain name

DeCent-Core can operate over any network, public or private. If exposing DeCent-Core to a public network, like the Internet, it's highly recommended to wrap the connection in a VPN or a trustworthy localhost-forwarding service.

## Open Source
The DeCent-Core codebase will be open-sourced shortly. Currently the codebase is undergoing some cleanup and refactoring from the prototype before release. 

In the meantime, if you're interested in implementing your own DCNT-compatible server, the protocol documentation should be enough to get you started.

## Downloads
DeCent-Core executables

- Windows: <a href="https://filebin.net/6p9g2amgpf6v1apg/DeCent-Core.zip" target="_blank">https://filebin.net/6p9g2amgpf6v1apg/DeCent-Core.zip </a>
- Linux: Coming soon
- Android: Coming soon


## Planned Features

Some of the features planned for future releases:

- Mutual TLS authentication option for incoming connections
- Integrated STUN server for a completely private signaling stack
- HTTP Authentication support for restricting server access
- Allowlist/blocklist for remote connections
- Let's Encrypt integration for trusted certificate generation and management
- DNS management integration for easy domain addressing
- Optional configuration and database encryption
- Improved certificate keystore/truststore management
- UI bug fixes
- Improved documentation
- More code samples

<br>



