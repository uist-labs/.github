# UIST Labs

A small, independent AI/ML lab. We build open tooling and publish certified,
quantized open-model checkpoints - held to a stated accuracy bar before they ship.

- Website: https://www.uistlabs.com
- Models on Hugging Face: https://huggingface.co/uist-labs

## What we do

**Certified quantization.** We quantize open models and publish a checkpoint only
after it clears a hard, stated accuracy gate against its full-precision baseline -
measured on the identical evaluation harness, with the real deltas published
alongside. A checkpoint that misses the bar doesn't ship. The name of the pipeline
behind it says the idea plainly: an *assay* is the test that certifies a refined
metal's purity.

**Runs on constrained hardware.** The checkpoints are weight-only NVFP4: they run
via vLLM's Marlin FP4 kernel with no Blackwell GPU required, validated down to
Ada-generation (sm_89) cards like the L4. Certified accuracy that travels to the
hardware you already have, not the hardware you would have to buy.

## Open projects

- **[assay](https://github.com/uistlabs/assay)** - the Apache-2.0 NVFP4 quantize ->
  benchmark -> gate -> publish pipeline behind every checkpoint we release.
- **[beautifulyze](https://github.com/uistlabs/beautifulyze)** - render a piece of
  music into a picture a language model can read.
- **[cogito](https://github.com/uistlabs/cogito)** - an experimental framework for
  exploring autonomous AI cognition through recursive self-prompting.

## How we work

- **Security first.** We don't trade security for convenience without saying so.
- **Trust, but verify.** Vendor claims are a starting point; the measured numbers
  are the product.
- **Standard tools, honest docs.** We prefer well-understood approaches, and we
  document the trade-offs, including what a release deliberately *doesn't* do.
