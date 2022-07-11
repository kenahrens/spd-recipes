# Recipes
## Environment Prep

Unzip to a directory, and open in your favorite editor.

- Make a copy of `default.env` and save for your testing (ex: `dev.env`)
- Populate the values inside `dev.env` from your `~/.speedscale/config.yaml` file
- Edit `docker-proxy-capture.yml` and modify:
    - `volumes` should point to the location where the `tls.key` and `tls.crt` can be found
    - `APP_LABEL` if you want to change the service name that will be shown in the Speedscale Traffic Viewer.

<aside>
⚠️ The compose files want to know which environment to use, you can set by using export like `export CONFIG=dev`

</aside>