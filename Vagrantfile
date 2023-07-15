projects=[
  "ctfd",
  "lumen",
  "ghidra"
]
Vagrant.configure("2") do |config|
  projects.each do |project|
    config.vm.define project do |node|
      node.vm.box = "ubuntu/jammy64"
      node.vm.hostname = project
      node.vm.provision "ansible" do |ansible|
      ansible.playbook = project+"/playbook.yml"
        ansible.become = true
        ansible.compatibility_mode = "2.0"
        ansible.extra_vars = {
          local: true
        }
      end
    end
  end
end