project('proj', 'c', default_options: ['warning_level=everything', ]
  )

glfw_dep = dependency('glfw3')
glad_dep = declare_dependency(
  sources: files('glad/glad.c'),
  include_directories: include_directories('glad'),
  compile_args: ['-Wno-everything'],
)

executable('program_executable',
  'src/main.c',
  dependencies: [glfw_dep, glad_dep],
  c_args: ['-g']
)
