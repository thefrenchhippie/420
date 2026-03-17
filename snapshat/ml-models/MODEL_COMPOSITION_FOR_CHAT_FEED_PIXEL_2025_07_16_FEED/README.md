# MODEL_COMPOSITION_FOR_CHAT_FEED_PIXEL_2025_07_16_FEED.prfb

## Model Card

Weights: uint8
LUT: included
Parameters: 976826 (1M)

## Architecture

Layer 0: CONV  /downs.0/downs.0.0/Conv
         Shape [16, 3, 6, 6] → kernel 6×6, stride 2, padding 2
         Weights: 1,728 uint8 + 16 float16 bias + 1024B LUT (f104.f5)

Layer 1: RELU  /downs.0/downs.0.2/Relu

Layer 2: CONV  /downs.1/residual/residual.0/Conv
         Shape [48, 16, 1, 1] → pointwise 1×1
         Weights: 1,536B float16
