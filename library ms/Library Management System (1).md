# 📚 Library Management System

**Day 1**

## Issue an item

[ ] Available only

OOP concepts used in this site's code

**Abstraction:** `LibraryItem`, `Member` cannot be instantiated (`new.target` check). **Encapsulation:** private `#status`, getters. **Inheritance:** single, multilevel (Book→ReferenceBook), hierarchical (Book/Magazine/DVD), multiple via the `Downloadable` mixin (EBook). **Polymorphism:** overridden `fine()`, `loanDays`, `canIssue`, `maxItems`, `fineFactor`; `search()` accepts a string or a year. **Static:** auto IDs and item count. **Composition:** `Loan` has an item and a member. **Generics:** `Repository`. **Exceptions:** `NotFoundError`, `LimitError` extend `LibraryError`. **Rules:** loan 14/7/3/21 days; limit 3 (student) / 5 (faculty); faculty pay 50% fine; unpaid fine blocks issuing.