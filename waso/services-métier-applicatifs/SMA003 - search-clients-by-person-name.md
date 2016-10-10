# BS003 searchClientsByPersonName

## Blocks

- Client
- Person

## Information System Services

- ISS004
- ISS005
- ISS002

## Input

- `personName`
- (`city`)

## Output

- `List<Client, List<Person>>`

## Description

Returns a list of the clients who have a person whose name is matching the
supplied `personName`. For each matching client, it also returns its list of
associated persons.

## Algorithm

- Use `getPersonsByName(personName)` [ISS004] to get a list of Persons
- For each Person in the response:
  - Use `getClientsByPersonId(Person.id)` [ISS005] to get a list of Clients
    with their list of personIds
    - For each item in the response:
      - For each personId in the list of personIds:
        - Use `getPersonById(personId)` [ISS002]
