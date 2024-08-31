# Retrieve all books
books = Book.objects.all()
print(books)

# Retrieve a specific book
book = Book.objects.get(title='1984')
print(book)
