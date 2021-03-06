# Qual ID - Contribution Guide

Qual ID welcomes contributions from people of all abilities. If you're new to open source software, then our issue to add data to existing categories is a _great first issue_.

If you're more experienced, or a newbie looking for something slightly more challenging, then our issue to add a new category is _perfect_.

## Add Data to an Existing Category

Adding data to a category essentially involves adding new strings to the list returned by the `get_values` method of a given category. Values must not contain any spaces or special characters, and must be appropriate to the given category. Once you've done this, simply raise a PR and it will be reviewed.

## Add a Brand New Category

Adding a new category involves adding a new class that inherits from the `Category` class. There are a few requirements for a successful PR:

- [ ] Add a new category class that inherits from `Category` class and overrides the `get_values` method.
- [ ] Add a new test class that asserts that the `get_values` method returns a list, and that all the values do not contain special characters or spaces.
- [ ] Add the new category to the `__category_map` in the pattern class, with the name of the category as the key, and an instance of your new category class as the value.

# Note

We request that for any contribution, at least 10 values are added, but of course the more the better!

# Thank You

Seriously, thank you for any contribution, we really appreciate it!
