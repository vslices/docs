# Methodology applied in Iteration 0

*How Domus Orbis used VSlices Method in its Iteration 0*

## Purpose

This document explains how VSlices Method was applied within Iteration 0 of Domus Orbis.

It does not aim to define a universal rule for all projects. It aims to show how a real case selected phases, documents, and *artifacts* according to its scope.

The beginning of Domus Orbis was an especially useful case because the initial problem was not mainly technical. The difficulty was preserving continuity between a real domestic need, a small solution, and a possible future evolution.

## General approach

The applied methodology followed a simple sequence:

{% include-markdown "shared/simple-design-iteration-flow.md" %}

Each phase produced only the documents or *artifacts* needed to support the next decision.

The objective was not to complete an ideal template. The objective was to preserve enough intention to build something small without losing the original problem.

## Why start with Iteration 0

Domus Orbis did not start with Iteration 1 because it was not yet clear what the first stable behavior should be.

Before defining the first Slice-First, it was necessary to document the current reality:

* where the need appeared
* which part of the scenario mattered
* which process was failing
* which terms could become important
* which small solution could reduce friction without solving the whole system

That is why Iteration 0 was used to understand and delimit.

The observed rule was:

> Iteration 0 documents the current reality. Iteration 1 defines the first stable Slice-First behavior.

## Small, not disposable Slice-First

The initial solution in Domus Orbis was small: a YAML file.

But that does not mean it was disposable.

The intention was to create an *artifact* that could survive future iterations. Even if command-line tools, automatic cart preparation, or market integrations exist later, the system will still need to know which products should be purchased, from which market, and in what quantity.

A good Slice-First is not the smallest possible code or *artifact*. It is the smallest stable behavior that protects the current need.
