Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"

  if Vagrant.has_plugin?('vagrant-proxyconf')
    config.proxy.http     = 'http://proxy.hoge.com:8080'
    config.proxy.https    = 'http://proxy.hoge.com:8080'
    config.proxy.no_proxy = 'localhost,127.0.0.1'
    config.proxy.enabled  = { pear: false }
  end

  config.vm.define 'docker' do |docker|
    docker.vm.hostname = 'docker'
    config.vm.provision :docker
    config.vm.provision :docker_compose
  end
end
