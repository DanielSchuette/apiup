# API Template

Creates a new Rails API pre-configured for JSON API and OAuth 2 authentication:

- Configures JSONAPI::Resources for JSON API
- Configures Doorkeeper for OAuth 2 authentication
- Creates a User model with `has_password` for password storage
- Sets up a `POST /users` endpoint for registration
- Configures FactoryBot factories for User and access tokens to make request specs easy
- Passes the `current_user` to JSONAPI::Resources

Also includes the following setup:

- Enables Rails API mode
- Removes Action Cable, Active Storage, Bootsnap, JBuilder, Spring, and Turbolinks
- Uses Postgres instead of SQLite
- Uses RSpec instead of Minitest
- Uses pry instead of byebug
- Disables authenticity token
- Enables CORS
- Adds:
  - Bullet
  - Dotenv
  - Factory Bot
  - Faker
  - Rack-Attack
- Provides a `Dockerfile` in case you want to run in Docker

To learn more, see ["Authorizing jsonapi_resources"](https://www.bignerdranch.com/blog/authorizing-jsonapi-resources-part-1-visibility/).

## Usage

Download the repo, then run `bin/apiup NEW-APP-NAME`.

To be able to run `apiup` from anywhere, add the repo's `bin` directory to your `PATH`.

## Thanks

Based on [this blog post](http://iamvery.com/2015/02/17/rails-new-for-you.html) by [iamvery](https://github.com/iamvery).

## License

Apache-2.0. See `License.txt` for details.
