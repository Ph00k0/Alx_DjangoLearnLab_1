# Retrieve the book
book = Book.objects.get(title='Nineteen Eighty-Four')

# Delete the book
book.delete()

# Verify the deletion
books = Book.objects.all()
print(books)
