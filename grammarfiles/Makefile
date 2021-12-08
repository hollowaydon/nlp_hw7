noisy_2.far: noisy_2.grm noisy.far byte.far entrain.sym
	thraxcompiler --save_symbols --input_grammar=$< --output_far=$@

noisy.far: noisy.grm byte.far entrain.fst entrain.sym entrain.alpha entrain.alpha
	thraxcompiler --save_symbols --input_grammar=$< --output_far=$@

byte.far: byte.grm 
	thraxcompiler --save_symbols --input_grammar=$< --output_far=$@

clean:
	rm -f noisy.far byte.far
