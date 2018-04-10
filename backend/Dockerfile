FROM elixir:1.6
RUN mix local.hex --force \
 && mix local.rebar --force \
 && mix archive.install https://github.com/phoenixframework/archives/raw/master/phx_new.ez --force
RUN apt update && apt install inotify-tools -y
WORKDIR /app
CMD ["iex"]
