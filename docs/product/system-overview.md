# System Overview

## System philosophy

Stable core + flexible edges.

## Core services

mpd
Audio playback engine.

playerd
System orchestrator.

inputd
Hardware input handler.

uid
User interface.

sysd
System services.

## Architecture diagram

```mermaid
graph TD

inputd --> playerd
uid --> playerd
playerd --> mpd
playerd --> sysd
playerd --> plugins
