# MAC (Multiply-Accumulate) Unit Design Specification

## Objective

The MAC unit performs multiplication of two input operands and accumulates the result into an internal accumulator register. It serves as the basic computational block of the systolic array matrix multiplication accelerator.

---

## Functional Description

The MAC performs the following operation:

ACC = ACC + (A × B)

The accumulator is cleared using a dedicated clear signal.

---

## Parameters

DATA_WIDTH

ACC_WIDTH

---

## Inputs

clk

rst

en

clr

a

b

---

## Outputs

acc

---

## Internal Registers

Accumulator Register

---

## Future Integration

This MAC will later become the Processing Element (PE) of the systolic array.
