This is a simple git repository for managing various forked MARC record related PHP libraries. These libraries were all originally provided via PEAR, and have been becoming
increasingly obsolete and unsupported for many years. They are still useful for anybody needing to handly MARC record creation or parsing.

The objective for each submodules is simply to keep the library working without throwing errors or warnings in PHP8.2+. Changes will naturally be incompatible with PHP7.4,
and probably incompatible with PHP8 to 8.1.

No functionality per se is provided through this repository.

#### Using the redcuillin forks in your project

One or more of the submodules can be added via composer in the following way:

    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/redcuillin/File_MARC"
        },
        {
            "type": "vcs",
            "url": "https://github.com/redcuillin/Validate_ISPN"
        },
        {
            "type": "vcs",
            "url": "https://github.com/redcuillin/Validate"
        },
        {
            "type": "vcs",
            "url": "https://github.com/redcuillin/php-marc"
        },
        {
            "type": "vcs",
            "url": "https://github.com/redcuillin/php-marc-spec"
        }
    ],
    "require": {
        "ck/php-marcspec": "dev-master as 2.999.0",
        "pear/file_marc": "dev-PHP8.4+-support",
        "pear/validate_ispn": "dev-master",
        "pear/validate": "dev-master",
        "scriptotek/marc": "dev-main"
    }

**Test carefully before using in production environments.**
