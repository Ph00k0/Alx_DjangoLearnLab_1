# Django Admin Interface Configuration for Book Model

## Steps to Register the Book Model

1. Open `bookshelf/admin.py` and add the following code:

   ```python
   from django.contrib import admin
   from .models import Book

   class BookAdmin(admin.ModelAdmin):
       list_display = ('title', 'author', 'publication_year')
       search_fields = ('title', 'author')
       list_filter = ('publication_year',)

   admin.site.register(Book, BookAdmin)
