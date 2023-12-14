# Xen Guest Agent systemd-sysext Extension

This repository contains a systemd-sysext compatible extension for the Xen Guest Agent, specifically designed for CoreOS/Flatcar Linux environments.

## Compatibility

The extension is compatible with systems that have an `ID` of `coreos` or an `ID_LIKE` of `coreos` in their `os-release`. It has been tested with Flatcar Container Linux and should work with other CoreOS derivatives.

## Installation and Usage

To use this extension with your CoreOS/Flatcar Linux system, follow these steps:

1. **Download the Latest Release**: 
   Download the latest release of the Xen Guest Agent extension from the GitHub repository's releases page.

2. **Install the Extension**:
   Copy the downloaded file to the `/etc/extensions` directory on your CoreOS/Flatcar system.

3. **Enable the Extension**:
   Run the following command to enable the extension:
   ```bash
   systemd-sysext refresh```

4. **Start the Service**:
   Once the extension is enabled, start the Xen Guest Agent service:
   ```bash
   systemctl start xen-guest-agent.service```

5. **Verify the Installation**:
   Verify that the service is running correctly:
   ```bash
   systemctl status xen-guest-agent.service```

## Contributing

Contributions to improve the Xen Guest Agent extension are welcome. Please submit issues and pull requests through the GitHub repository.

## License

This project is licensed under the [GNU General Public License v3.0](LICENSE).

## Support

For support and bug reports, please submit an issue on the GitHub repository's issue tracker.
