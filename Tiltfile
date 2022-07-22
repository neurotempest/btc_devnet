# -*- mode: Python -*-

docker_build(
  ref='bitcoind_localnet',
  context='.',
  dockerfile='deployments/Dockerfile.bitcoind',
)

k8s_yaml('deployments/bitcoind_localnet.yml')
