Vagrant.configure(2) do |config|
  config.vm.box = "kjkuhn/ubuntu2004"
  config.vm.box_version = "0.0.1"

  config.vm.network :forwarded_port, guest: 50022, host: 50222

  config.vm.provider "qemu" do |qe|
    qe.arch = "x86_64"
    qe.machine = "q35"
    qe.cpu = "max"
    qe.net_device = "virtio-net-pci"
  end
end