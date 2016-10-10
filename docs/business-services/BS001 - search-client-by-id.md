# BS001 searchClientById

## Blocks

- Client
- Person

## Information System Services

- ISS001 - getClientById
- ISS002 - getPersonById

## Input

- `clientId`
- (`city`)

## Output

- `Client`
- `List<Person>`

## Description

Returns the client corresponding to the supplied `clientId` with the list of
associated persons.

## Algorithm

- Use `getClientById(clientId)` [ISS001] to get Client and personIdList
- For each personId in personIdList:
  - Use `getPersonById(personId)` [ISS002]
