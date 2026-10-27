# AuthCove

**Secure authentication, clear consent, and private sessions.**

AuthCove is an independent Customer Passport and OpenID Connect provider. Participating products let their customers sign in with one AuthCove Passport, while each product keeps its own user mapping, authorization data, and browser session.

## What it does

- **Sign-in** with Google, plus Passkeys bound to your Passport
- **OpenID Connect** Authorization Code flow with S256 PKCE
- **Clear consent**: users confirm which Passport to use and can review and manage connected applications
- **Brand-neutral issuer**: `https://authcove.com`

## For integrators

1. Request a pre-registered OIDC client and an exact redirect URI from the AuthCove operator.
2. Discover endpoints from [`/.well-known/openid-configuration`](https://authcove.com/.well-known/openid-configuration).
3. Implement Authorization Code with S256 PKCE and validate the returned ID token.
4. Map `issuer + sub` to your local customer and create your own session.

## Links

- Website: [authcove.com](https://authcove.com)
