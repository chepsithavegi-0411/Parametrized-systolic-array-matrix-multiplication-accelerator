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

clk  : it used to provide clock for sequential logic in MAC units and ensures synchronized operation

rst  : used when we need to perform new matrix multiplication operation . it reinitializes the design

en   : it is used for stoping the processing units from performing unnecessary calculations during the operation. when en = 0 the accumulator hold its current value

clr  : clears the internal accumulator register so a new accumulation can begin without resetting the entire module.

a    : it is an innput operand from MATRIX A

b    : it is an input operand from MATRIX B

---

## Outputs

acc

---

## Internal Registers

Accumulator Register

---

## Future Integration

This MAC will later become the Processing Element (PE) of the systolic array.
