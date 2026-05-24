<div align="center">

# Composer Audit to SARIF Action

[![GitHub Release](https://img.shields.io/github/v/release/typisttech/composer-audit-to-sarif-action)](https://github.com/typisttech/composer-audit-to-sarif-action/releases/latest)
[![GitHub Marketplace](https://img.shields.io/badge/marketplace-php--matrix-blue?logo=github)](https://github.com/marketplace/actions/php-matrix)
[![Test](https://github.com/typisttech/composer-audit-to-sarif-action/actions/workflows/test.yml/badge.svg)](https://github.com/typisttech/composer-audit-to-sarif-action/actions/workflows/test.yml)
[![License](https://img.shields.io/github/license/typisttech/composer-audit-to-sarif-action.svg)](https://github.com/typisttech/composer-audit-to-sarif-action/blob/master/LICENSE)
[![Follow @TangRufus on X](https://img.shields.io/badge/Follow-TangRufus-15202B?logo=x&logoColor=white)](https://x.com/tangrufus)
[![Follow @TangRufus.com on Bluesky](https://img.shields.io/badge/Bluesky-TangRufus.com-blue?logo=bluesky)](https://bsky.app/profile/tangrufus.com)
[![Sponsor @TangRufus via GitHub](https://img.shields.io/badge/Sponsor-TangRufus-EA4AAA?logo=githubsponsors)](https://github.com/sponsors/tangrufus)
[![Hire Typist Tech](https://img.shields.io/badge/Hire-Typist%20Tech-778899)](https://typist.tech/contact/)

<p>
  <strong> Convert Composer audit reports to SARIF files</strong>
  <br>
  <br>
  Built with ♥ by <a href="https://typist.tech/">Typist Tech</a>
</p>

</div>

---

> [!TIP]
> **Hire Tang Rufus!**
>
> I am looking for my next role, freelance or full-time.
> If you find this tool useful, I can build you more dev tools like this.
> Let's talk if you are hiring PHP / Ruby / Go developers.
>
> Contact me at https://typist.tech/contact/

---

## Usage

See [action.yml](action.yml) and the underlying script [`ComSARIF`](https://github.com/typisttech/comsarif/#options).

```yaml
  - uses: typisttech/composer-audit-to-sarif-action@0
    with:
      # Path to Path to audit JSON file
      #
      # Default: audit.json
      audit: some/path/to/audit.json

      # Path to composer.lock
      #
      # Default: composer.lock
      lock: some/path/to/composer.lock

      # Path to repository root
      #
      # Default: ${{ github.workspace }}
      root: some/path

      # ComSARIF version.
      #
      # The version of [ComSARIF] to use. Leave blank for latest. For example: v1.0.2
      #
      # [ComSARIF]: https://github.com/typisttech/comsarif
      #
      # Default: ''
      version: v1.0.2

      # Verify Attestation
      #
      # Whether to verify ComSARIF tarball attestation.
      #
      # Default: true
      verify-attestation: false

      # Github Token
      #
      # GitHub token to use for authentication
      #
      # Default: ${{ github.token }}
      github-token: ${{ secrets.GITHUB_PAT_TOKEN }}
```

### Outputs

| Key | Description | Example |
| --- | --- | --- |
| `sarif`  | Path to the SARIF file | `/tmp/comsarif-123.sarif` |

> [!TIP]
> **Hire Tang Rufus!**
>
> There is no need to understand any of these quirks.
> Let me handle them for you.
> I am seeking my next job, freelance or full-time.
>
> If you are hiring PHP / Ruby / Go developers,
> contact me at https://typist.tech/contact/

## Examples

<details open>
  <summary>TODO</summary>

```yaml
TODO
```
</details>

## Credits

[`Composer Audit to SARIF Action`](https://github.com/typisttech/composer-audit-to-sarif-action) is a [Typist Tech](https://typist.tech) project and
maintained by [Tang Rufus](https://x.com/TangRufus), freelance developer [for hire](https://typist.tech/contact/).

Full list of contributors can be found [on GitHub](https://github.com/typisttech/composer-audit-to-sarif-action/graphs/contributors).

## Copyright and License

This project is a [free software](https://www.gnu.org/philosophy/free-sw.en.html) distributed under the terms of
the MIT license. For the full license, see [LICENSE](LICENSE).

## Contribute

Feedbacks / bug reports / pull requests are welcome.
