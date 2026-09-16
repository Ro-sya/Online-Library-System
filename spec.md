# Online Library System

## 1. Опис сутностей та атрибутів

- **Reader:** `id` (uuid), `ticket_number` (string), `full_name` (string), `email` (string), `created_at` (datetime).
- **Book:** `id` (uuid), `title` (string), `book_number` (string), `year` (int).
- **Author:** `id` (uuid), `full_name` (string), `country` (string).
- **Genre:** `id` (int), `name` (string). 
- **Digital Access:** `id` (uuid), `reader_id` (uuid), `book_id` (uuid), `granted_at` (datetime), `expires_at` (datetime), `is_active` (boolean).

## 2. Зв'зки між сутностями

- `Book` - `Author` (N:1)
- `Reader` - `Digital Access` (1:N)
- `Book` - `Genre` (N:M)
- `Book` - `Digital Access` (1:N)

## 3. Mermaid ER-Diagram
