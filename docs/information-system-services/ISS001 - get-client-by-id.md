# ISS001 getClientById

## Block

Client

## Entities

- Client

## Input

- `clientId`

## Output

- `Client`
- `List<personId>`
- `walletId`
- `structureElementId`

## Description

Retrieve the Client identified by the provided `clientId` and the list of IDs
of the associated persons. Also returns the ID of the wallet containing this
client and the ID of the structure handling the client.
