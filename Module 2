def display_menu():
    print('Contact Manager')
    print()
    print('COMMAND MENU')
    print('list    - Display all contacts')
    print('view - View a contact')
    print('add   - Add a contact')
    print('del    - Delete a contact')
    print('exit   - Exit program')
    print()

def lists(contact_list):
    if len(contact_list) == 0:
        print('There are no contacts in the list.\n')
        return
    else:
        i=1
        for contact in contact_list:
            print(str(i) + '. ' + contact[0])

def view(contact_list):
    number = int(input('Number: '))
    if number < 1 or number > len(contact_list):
        print('Invalid contact number.\n')
    else:
        contact = contact_list[number-1]
        print('Name: ' + contact[0])
        print('Email: ' + contact[1])
        print('Phone: ' + contact[2])
    
def add(contact_list):
    name = input('Name: ')
    email = input('Email: ')
    phone = input('Phone: ')
    contact = []
    contact.append(name)
    contact.append(email)
    contact.append(phone)
    contact_list.append(contact)
    print(name + ' was added.\n')
      
def delete(contact_list):
    number = int(input('Number: '))
    if number < 1 or number > len(contact_list):
        print('Invalid contact number.\n')
    else:
        contact = contact_list.pop(number-1)   
        print(contact[0] + ' was deleted.\n')
        
def main():
    contact_list = [['Marilyn Monroe', 'MarilynMonroe@whitehouse.org', '+22 33 4567 4587'],
                    ['Abraham Lincoln','AbrahamLincoln@whitehouse.org','+22 33 4567 4587']]
    display_menu()
    
    while True:
        command = input('Command: ')
        if command.lower() == 'list':
            lists(contact_list)
        elif command.lower() == 'view':
            view(contact_list)
        elif command.lower() == 'add':
            add(contact_list)
        elif command.lower() == 'del':
            delete(contact_list)
        elif command.lower() == 'exit':
            break
        else:
            print('That is not a valid command. Please try again.\n')
    print('Bye!')

if __name__ == '__main__':
    main()    
