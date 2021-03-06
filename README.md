# NAME

Data::Object::Role::Dumpable

# ABSTRACT

Dumpable Role for Perl 5

# SYNOPSIS

    package Example;

    use Moo;

    with 'Data::Object::Role::Dumpable';

    package main;

    my $example = Example->new;

    # $example->dump

# DESCRIPTION

This package provides methods for dumping the object and underlying value.

# METHODS

This package implements the following methods:

## dump

    dump() : Str

The dump method returns a string representation of the underlying data.

- dump example #1

        # given: synopsis

        my $dumped = $example->dump;

## pretty\_dump

    pretty_dump() : Str

The pretty\_dump method returns a string representation of the underlying data
that is human-readable and useful for debugging.

- pretty\_dump example #1

        # given: synopsis

        my $dumped = $example->pretty_dump;

## pretty\_print

    pretty_print(Any @args) : Int

The pretty\_print method prints a stringified human-readable representation of
the underlying data.

- pretty\_print example #1

        # given: synopsis

        my $printed = $example->pretty_print;

- pretty\_print example #2

        # given: synopsis

        my $printed = $example->pretty_print({1..4});

## pretty\_say

    pretty_say(Any @args) : Int

The pretty\_say method prints a stringified human-readable representation of the
underlying data, with a trailing newline.

- pretty\_say example #1

        # given: synopsis

        my $printed = $example->pretty_say;

- pretty\_say example #2

        # given: synopsis

        my $printed = $example->pretty_say({1..4});

## print

    print(Any @args) : Int

The print method prints a stringified representation of the underlying data.

- print example #1

        # given: synopsis

        my $printed = $example->print;

- print example #2

        # given: synopsis

        my $printed = $example->print({1..4});

## say

    say(Any @args) : Int

The say method prints a stringified representation of the underlying data, with
a trailing newline.

- say example #1

        # given: synopsis

        my $printed = $example->say;

- say example #2

        # given: synopsis

        my $printed = $example->say({1..4});

# AUTHOR

Al Newkirk, `awncorp@cpan.org`

# LICENSE

Copyright (C) 2011-2019, Al Newkirk, et al.

This is free software; you can redistribute it and/or modify it under the terms
of the The Apache License, Version 2.0, as elucidated in the ["license
file"](https://github.com/iamalnewkirk/data-object-role-dumpable/blob/master/LICENSE).

# PROJECT

[Wiki](https://github.com/iamalnewkirk/data-object-role-dumpable/wiki)

[Project](https://github.com/iamalnewkirk/data-object-role-dumpable)

[Initiatives](https://github.com/iamalnewkirk/data-object-role-dumpable/projects)

[Milestones](https://github.com/iamalnewkirk/data-object-role-dumpable/milestones)

[Contributing](https://github.com/iamalnewkirk/data-object-role-dumpable/blob/master/CONTRIBUTE.md)

[Issues](https://github.com/iamalnewkirk/data-object-role-dumpable/issues)
