---
tags: php, laravel, laravel-routes
---

# routes/web php

> meant to define the routes for the web app

## example

```php
<?php
// "include" classes, Route is default
use Illuminate\Support\Facades\Route;
use App\Http\Controllers\TodoListController;

// define the routes (get, post, put, up, patch, delete, options)
Route::get('/', [TodoListController::class, 'index']);
Route::get('/completed', [TodoListController::class, 'completed']);
Route::post('/saveItem', [TodoListController::class, 'saveItem'])->name('saveItem');
/>
```
