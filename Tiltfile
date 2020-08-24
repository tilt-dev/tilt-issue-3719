docker_build('example-html-image', '.')
k8s_yaml('deployment.yaml')
k8s_resource('example-html', port_forwards=8000)

if config.tilt_subcommand == 'up':
  k8s_yaml('config.yaml')
  k8s_yaml('pvc.yaml')
