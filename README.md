# pblink-proto

Single Source of Truth protocol definitions, topic mappings, and custom Protobuf control messages for the `pblink` ecosystem.

## Overview
This repository contains:
- `topics.yaml`: Central registry of uORB topic mappings, message type IDs, and default streaming rates (Hz).
- `proto/`: Protocol Buffer schemas (`.proto`) for administrative handshake, dynamic rate adjustment, parameter inspection, and time synchronization.

## Schema Components
- **`subscription_request.proto`**: Dynamic topic rate adjustment request.
- **`time_sync.proto`**: High-precision time synchronization between PX4 and Companion.
- **`parameter_request.proto` / `parameter_set.proto` / `parameter_value.proto`**: Parameter read/write RPCs.
- **`topic_list_response.proto`**: Dynamic topic discovery response.
