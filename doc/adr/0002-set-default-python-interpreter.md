# 2. Set default python interpreter

Date: 2025-03-01

## Status

Accepted

## Context

The issue motivating this decision, and any context that influences or constrains the decision.
[WARNING]: Platform linux on host spark is using the discovered Python interpreter at /usr/bin/python3.11, but future
installation of another Python interpreter could change the meaning of that path. See https://docs.ansible.com/ansible-
core/2.18/reference_appendices/interpreter_discovery.html for more information.

## Decision

Add to ansible config defaults

[defaults]
interpreter_python = /usr/bin/python3

## Consequences

May be need to adjust it more specific in future