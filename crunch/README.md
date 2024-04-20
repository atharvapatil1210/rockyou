# crunch password generator

#### install Crunch

        crunch <min_length> <max_length> [options] -o <output_file>

<min_length>: The minimum length of passwords to generate.

<max_length>: The maximum length of passwords to generate.

<output_file>: Specify the output file where the generated passwords will be saved.

Generate Passwords:

        crunch <min_length> <max_length> [options] -o <output_file>

For example, to generate all possible alphanumeric passwords of length 6:

        crunch 6 6 -o passwords.txt

You can also specify character sets using -t option. For example, to generate passwords with uppercase letters and numbers:

        crunch 6 8 -t @%^&0123456789 -o passwords.txt

Options:

    -f <file>: Specify a file containing character sets to use for password generation.
    -t: Specify a custom character set directly in the command.
    -d <digits>: Specify the number of digits to use in generated passwords.
    -s <symbols>: Specify the number of symbols to use in generated passwords.