# StateHasChangedValidation

This repository contains a sample application and test evidence used to validate
the analyzer diagnostics for unnecessary `StateHasChanged` calls in ASP.NET Core
issue #68484.

## Repository Structure

### StateHasChangedSample

A .NET 11 Blazor sample application in interactive server mode used to verify that unnecessary
`StateHasChanged` calls produce `BL0012` warnings, while genuinely necessary calls
do not produce warnings.

### Evidence

Contains screenshots, recordings, and other evidence collected during validation.

## Purpose

The repository provides:

- A .NET 11 validation sample.
- IDE and command-line analyzer evidence.
- Runtime evidence before and after applying the fixes.

## Issue

[#68484: "[Validation] Analyzer diagnostics for unnecessary StateHasChanged calls"](https://github.com/dotnet/aspnetcore/issues/68484).