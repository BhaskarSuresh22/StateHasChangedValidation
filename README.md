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
- IDE evidence and compact command-line build logs.
- Build logs containing the commit hash, SDK version, `BL0012` warning
	count, and individual analyzer diagnostics for each validated revision.
- Runtime evidence before and after applying the fixes.

## Revision State

The current `main` branch is intentionally back on the four-warning scenario and
does not represent the final fixed source. The final fixed state is preserved in
the historical [`26f6262`](https://github.com/BhaskarSuresh22/StateHasChangedValidation/commit/26f6262)
revision. Check out that revision to inspect or reproduce the version in which
the four unnecessary `StateHasChanged` calls were removed.

## Issue

[#68484: "[Validation] Analyzer diagnostics for unnecessary StateHasChanged calls"](https://github.com/dotnet/aspnetcore/issues/68484).