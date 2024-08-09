# Delete a Book Instance

**Command:**

```python
from bookshelf.models import Book

# Retrieve the book instance (assuming it's the one created earlier)
book = Book.objects.get(title="Nineteen Eighty-Four")

# Delete the book instance
book.delete()
