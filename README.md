# nuxt-xp-oidc

Example project integrating [authentik](https://goauthentik.io/) and [nuxt](https://nuxt.com/) using [nuxt-oidc-auth](https://nuxt.com/modules/nuxt-oidc-auth).

nuxt-oidc-auth does not (yet) have a native authentik provider profile. This example illustrates how to set up a generic oidc config for it.

Tested with:

* Nuxt 3.12.4
* nuxt-oidc-auth 0.12.0

Check `nuxt.config.ts` for configuration options.

> Change the URLs to fit your authentik (or other oidc) provider.

Basic usage is showcased in `pages/index.vue` and `pages/auth/login.vue`