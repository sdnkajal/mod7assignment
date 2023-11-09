# মডিউল ৭ এর এসাইনমেন্ট
## Assignment - Laravel Structure and Artisan Commands
### Objective:
In this assignment, you will create a basic Laravel application and use artisan commands to generate controllers and routes

### Task:
- Create a new Laravel application using the command line. Use the necessary Laravel installer command to create the project.
```shell
composer create-project laravel/laravel mod7assignment
```
- Once the project is created, use the artisan command to generate a new controller called 'UserController'.
```shell
php artisan make:controller UserController
```
- Next, create a route in the web.php file that maps to a function in the UserController. The function should return a simple message like 'Hello, Laravel!'.
```php
// File name: web.php
Route::get('/users', [UserController::class, 'index']);


// File name: UserController.php
namespace App\Http\Controllers;
use Illuminate\Http\Request;
class UserController extends Controller
{
    public function index(): string
    {
        return "Hello, Laravel!";
    }
}
```
- Finally, start the Laravel development server and test the route using a web browser.
```php
php artisan serve
```


### Criteria:
- The Laravel project should be created successfully using the correct artisan command.
- The UserController should be generated using the appropriate artisan command.
- The route in the web.php file should be configured correctly and mapped to the UserController function.
- The UserController function should return the expected message.
- The route should be accessible and displaying the expected message when tested in a web browser.

### Hint:
Refer to the Laravel documentation and online tutorials for guidance on creating a new Laravel application and using artisan commands.

### Submission Guidelines:
1. Must Submit Github link
2. Must Create a Fresh New Repository and this repository should have only laravels folders and files.
3. Don't push a folder where your project is created. So that we don't need to go inside that folder.
4. Demo: https://drive.google.com/file/d/19B1kkA5oGWe6aUIjI1lAdZsEyoJZfX6U/view?usp=sharing
