# mobile-names-and-numbers
#based on python creation of reposotory if students and numbers
names = []
phone_numbers = []
num = 30


for i in range(num):
    name = input("Name: ")
    phone_number = input("Phone Number: ") 
    names.append(name)
    phone_numbers.append(phone_number)

print("\nName\t\t\tPhone Number\n")

for i in range(num):
    print("{}\t\t\t{}".format(names[i], phone_numbers[i]))

search_term = input("\nEnter search term: ")

print("Search result:")

if search_term in names:
    index = names.index(search_term)
    phone_number = phone_numbers[index]
    print("Name: {}, Phone Number: {}".format(search_term, phone_number))

else:
    print("Name Not Found")
