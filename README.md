usage: transeq [-h] [-v {short,long}] [-p {1,2}] [-r] [-s STOP_CHARACTER]
               [--no_mask] [--keep_whitespace]
               [sequence_input]

Translate nucleotide sequence into amino acid sequence

positional arguments:
  sequence_input        sequence string or file containing sequence(s)
                        (default: None)

optional arguments:
  -h, --help            show this help message and exit
  -v {short,long}, --verbosity {short,long}
                        amino acid abbreviation length (e.g. Glu/Glutamine)
                        (default: single)
  -p {1,2}, --phase {1,2}
                        change the phase of translation (default: 0)
  -r, --reverse_complement
                        reverse-complement the sequence before translation
                        (default: False)
  -s STOP_CHARACTER, --stop_character STOP_CHARACTER
                        the string to use for stop codons (default: *)
  --no_mask             do not mask unrecognized codons with X; report
                        lowercased (default: False)
  --keep_whitespace, -k
                        treat whitespace (both bordering and internal) as
                        sequence (default: False)
