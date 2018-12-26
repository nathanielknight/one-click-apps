## Test Repo for CaptainDuckDuck V1 One Click Apps

Process:
- Find/create a docker-compose file for the one click app
- Convert yaml file to json
- Copy the content into the structure as `/one-click-apps/v1/wordpress.json`
- Variables are prefixed with `$$cap`
- There is one special variable called `$$cap_appname$$` which exists for all oneclick apps
- Varibles can be anywhere in the JSON and they will be replaced by what user enters
- Each variable must have `id`, `type`, `label`. It may also have `defaultValue`, `validRegex`, `description`.
- Other than `image`, `environment`, `ports`, `volumes`, `depends_on`, other parameters are ignored. Make sure they are not important.
