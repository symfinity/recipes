<div align="center">

# Recipes

### Custom Symfony Flex recipes tailored for **symfinity** branded Symfony packages

[![symfony/recipes](https://img.shields.io/badge/symfony-recipes-374151.svg?style=flat)](https://github.com/symfony/recipes)
[![symfony/recipes-contrib](https://img.shields.io/badge/symfony-recipes--contrib-374151.svg?style=flat)](https://github.com/symfony/recipes-contrib)

[![php](https://img.shields.io/badge/PHP-^8.1-4F5B93.svg?style=flat)](https://www.php.net)
[![composer](https://img.shields.io/badge/composer-^2.1-D48822.svg?style=flat)](https://getcomposer.org)
[![symfony](https://img.shields.io/badge/symfony/flex-^2-374151.svg?style=flat)](https://github.com/symfony/flex)

</div>

---

## Getting Started

This repository contains custom Symfony Flex recipes for **symfinity** packages. Recipe **sources** live on branch `main`; the Flex **endpoint** (generated `index.json`, vendor JSON files, `RECIPES.md`) lives on branch `flex/main`.

To enable recipes from this repository in your project, add this endpoint in your project's `composer.json` as described in the [Symfony documentation](https://symfony.com/doc/current/setup/flex_private_recipes.html#configure-your-project-s-composer-json-file):

```json
{
    "extra": {
        "symfony": {
            "endpoint": [
                "https://api.github.com/repos/symfinity/recipes/contents/index.json?ref=flex/main",
                "flex://defaults"
            ]
        }
    }
}
```

> [!WARNING]
> Without this option Composer will not use the Symfony Flex recipes for **symfinity** packages unless the recipes were contributed to [symfony/recipes-contrib](https://github.com/symfony/recipes-contrib).

> [!NOTE]
> See [RECIPES.md](https://github.com/symfinity/recipes/blob/flex/main/RECIPES.md) for a full list of recipes on the Flex endpoint branch.

## Contributing

Only authorized team members can contribute to this repository.

## Support

If you run into problems or have questions about the recipes, open an issue in the monorepo or contact the maintainers.

## License

This repository is experimental. Prefer [symfony/recipes-contrib](https://github.com/symfony/recipes-contrib) when recipes are accepted upstream.

## About

[symfinity.net](https://symfinity.net) — Symfony-first packages and tooling.

## Acknowledgements

Thanks to the Symfony community for recipes-contrib and Flex.

---

Copyright (c) 2026-present [symfinity.net](https://symfinity.net)
