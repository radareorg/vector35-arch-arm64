project('v35arm64', 'c', meson_version : '>=0.60.0', version : '2.0.2')

sources = [
  'disassembler/decode.c',
  'disassembler/decode0.c',
  'disassembler/decode1.c',
  'disassembler/decode2.c',
  'disassembler/decode_fields32.c',
  'disassembler/decode_scratchpad.c',
  'disassembler/encodings_dec.c',
  'disassembler/encodings_fmt.c',
  'disassembler/format.c',
  'disassembler/gofer.c',
  'disassembler/operations.c',
  'disassembler/pcode.c',
  'disassembler/regs.c',
  'disassembler/sysregs.c'
]

incs = include_directories(['disassembler'])
libs = both_libraries('v35arm64', sources)

v35arm64_dep = declare_dependency(
  link_with: [libs.get_static_lib()],
  include_directories: incs
)
