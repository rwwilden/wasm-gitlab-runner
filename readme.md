- Docker compose file with gitlab and gitlab runner
- Create empty config.toml for gitlab-runner
- Enter gitlab-runner container: `docker exec -it gitlab-runner bash`
- Register runner: `gitlab-runner register`
    - `http://gitlab:8929`
    - \<registration-token>
    - Rust WASM runner


- Clone on a different port:
  Instead of:
  git clone git@gitlab.rwwilden.com:gitlab-instance-87971b22/test-project.git
  do
  git clone ssh://git@gitlab.rwwilden.com:2289/gitlab-instance-87971b22/test-project.git