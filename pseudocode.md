# Pseudocode

## Classes:
Contact():
    - name (string)
    - phone_number (string)
    - email (Optional string)
    - address (Optional string)

Phonebook():
    - contacts (HashMap of String & Contact)

## Add a contact
function add_contact(name, phone_number, email, address):
    if (contacts.get(name) is present):
       error: contact already exists

    contacts.put(name) = Contact(name, phone_number, email, address)

## Remove a contact
function remove_contact(name):
    if (contacts.get(name) is not present):
       error: contact does not exist

    contacts.remove(name)


## View all contacts
function view_contacts():
    for contact in contacts:
        print(contact.name)
        print(contact.phone_number)
        print(contact.email)
        print(contact.address)

## Search for a contact
function search_contact(name):
    if (contacts.get(name) is not present):
       error: contact does not exist

    print(contacts.get(name).name)
    print(contacts.get(name).phone_number)
    print(contacts.get(name).email)
    print(contacts.get(name).address)
