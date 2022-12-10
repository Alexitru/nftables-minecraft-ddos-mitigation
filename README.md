# nftables Minecraft Server DDoS Mitigation Configuration

This repository contains an `nftables` configuration file with rules for protecting a Minecraft server from DDoS attacks. The configuration includes layer 7 filtering and specific rules for blocking common types of DDoS attacks, such as fake sessions, query floods, and bot attacks.

## Requirements

- An `nftables`-compatible firewall
- A Minecraft server running on port 25565

## Installation

To use this `nftables` configuration, follow these steps:

1. Clone or download this repository to your server.
2. Open the `nftables.conf` file in a text editor.
3. Review the rules and adjust any settings as needed, such as the IP addresses and port numbers.
4. Save the `nftables.conf` file.
5. Run the `nftables-apply` command to apply the configuration to your firewall.

## Usage

Once the configuration is applied, incoming and outgoing connections to the Minecraft server on port 25565 will be allowed, while malicious connections that use fake sessions, query floods, or bot attacks will be blocked. Additionally, the configuration includes filtering for IP addresses and port numbers, as well as rate limiting for incoming and outgoing connections.

## Troubleshooting

If you encounter any issues with the `nftables` configuration, you can try the following steps to troubleshoot and resolve the problem:

1. Check the `nftables` logs for any error messages or warnings.
2. Review the rules in the `nftables.conf` file to ensure they are correct and up-to-date.
3. Try disabling or adjusting the rate limiting rules to see if they are causing any issues.
4. If the problem persists, you can try restoring the default `nftables` configuration and reapplying the rules from this repository.

## Contributions

Contributions to this `nftables` configuration are welcome. If you have any suggestions for improvements or additional rules, you can open a pull request with your changes.

## License

This `nftables` configuration is released under the [MIT license](LICENSE).
