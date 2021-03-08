_Is your code not working? That is very normal, especially when you are first starting. Keep at it! You can work through any of the challenges you face on this "assignment"._

## General

Have questions related to assignment 0 in general? Look for them here!

#### "Learn Karel Basics" is not marked as complete

The step that consists of reading Chapters 1-5 doesn't get marked as complete with a green tick like the other steps. Feel free to read at your own pace and move on from this step when you finish the chapters.

#### I can't access my account anymore, or it's blank!

1. Navigate to the [Code In Place homepage](https://codeinplace.stanford.edu), reopen the application form, and try to sign in again.
2. Are you using a phone? Try logging in from a computer instead?
3. Try out any other email you might have signed up with.
4. Try both the "Sign in with email" and the "Sign in with Google" buttons. Depending on whether you originally selected "Sign in with email" or "Sign in with Google", there are some cases where trying to login with the opposite method will cause problems.
5. If all else fails: send us an email with screenshots/details about your problem. We'll do everything we can to make sure you don't lose any progress.

#### Have you received my application?

Sign into your student application and look for the green status bar at the top of the application. If it says "Application complete! You finished...", then we have successfully received your application! If your application isn't complete, that status bar will show what your next steps are.

## Understanding Typos

Reading error messages for typos is a skill that is worth learning but takes some practice. Here is a translation of some of the common ones and what they could mean.

#### `Expected a body definition`

All functions (like `main`) need to have a body, which is the indented code. See Chapter 3 of the Karel Reader. For example, in this `turn_right` fucntion definition, the `turn_left` commands are all in the body:

```
def turn_right():
    turn_left()
    turn_left()
    turn_left()
```

#### `Function body must be indented...`

All functions (like `main`) need to have a body, which is the indented code. See Chapter 3 of the Karel Reader. If you don't have any code in the function body, that can lead to this error.

#### `Found a newline when expecting ":"`

If you are defining a new function, or a for loop, you need to end that line of code with a `:` (a colon).

#### `Found "<something>" when expecting "("`

There are several issues that can cause this message.

1. Every command has open and close parentheses after it. So for example we write move(), not move. Similarly, when you define a function, you also write open and close parentheses after the name. You will learn why we do this in a few weeks!
2. This can happen if you try to declare a function inside another function. In Karel, that is not allowed. Recall that there is a difference between defining a new function and using one:

```
def main():
    move()
    def illegal_nested_function():
        turn_left()
```

#### `Found move when expecting def`

In Karel, all commands must be declared inside a function! Do you have a `main` function?

## Shelter-in-place

#### It's not being marked as complete.

Whenever a Karel program isn't being marked as complete when you think it should be, immediately see if any error messages are popping up below the Karel window. If this is the case, check out the "Understanding Typos" section.

If it isn't an error message, reread the exercise requirements. A common mistake with "Shelter-in-place" is returning the beeper to the starting point instead of just returning Karel to its starting point. To clarify- we don't want any beepers present in the world after our code runs for this problem.

## Piles

#### My `for` loop won't stop

The number after `range(` is the number of times the indented code underneath the `for` loop runs. In this example, any code you write in the code block where we've written `# Code that repeats`. repeats 11 times. If you would like the `for` loop to end earlier, you can use a smaller number. While there are other ways to stop a loop, this is the best strategy to do so for this problem. Check out Chapter 5 for more information!

```
for i in range(11):
    # code that repeats
```
