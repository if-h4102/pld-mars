# BS002 searchClientsByName

## Blocks

- Client
- Person

## Information System Services

- ISS002 - getPersonById
- ISS003 - getClientsByName

## Input

- `clientName`
- (`city`)

## Output

- `List<Client, List<Person>>`

## Description

Returns the list clients named `clientName` with the list of their
associated persons.

## Algorithm

## Algorithm

- Use `getClientsByName(clientName)` [ISS003] to get clients with their personIds
- For each client and list of personId in the response:
  - For each personId in personIdList:
    - Use `getPersonById(personId)` [ISS002]

