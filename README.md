# LSL\_Mindaffect\_guide: Integrating g.USBamp with MindAffect BCI via Lab Streaming Layer

This repository provides a step-by-step guide to integrating the g.USBamp EEG amplifier from g.tec with the MindAffect open-source Brain-Computer Interface (BCI) system using the Lab Streaming Layer (LSL) protocol. It includes configuration files, software setup instructions, and supplementary resources to facilitate the setup process.([youtube.com][1])

## Repository Contents

* **LaunchGuide.txt**: Text-based instructions outlining the setup process.
* **Software Guide.docx**: Detailed documentation with images to assist in software installation and configuration.
* **Updated-32.cfg**: Configuration file tailored for a 32-channel EEG setup.
* **gNEEDaccess.rar**: Compressed archive containing the g.NEEDaccess client/server software required for g.USBamp operation.
* **noisetag\_bci2.json**: Sample configuration file for the MindAffect BCI system.([github.com][2], [github.com][3])

## Prerequisites

Before proceeding with the setup, ensure you have the following:

* **g.USBamp EEG Amplifier**: Hardware device from g.tec for EEG signal acquisition.
* **g.NEEDaccess Software**: Client/server software provided by g.tec to interface with the g.USBamp.
* **Lab Streaming Layer (LSL) Streamer**: Software to stream EEG data from g.USBamp over LSL.
* **MindAffect BCI Software**: Open-source BCI framework that utilizes c-VEP stimuli for communication.([youtube.com][1], [bci.plus][4])

## Setup Instructions

1. **Download MindAffect BCI Software**:

   * Clone or download the MindAffect BCI repository:

     ```bash
     git clone https://github.com/mindaffect/pymindaffectBCI.git
     ```
   * Follow the installation instructions provided in the [MindAffect documentation](https://mindaffect-bci.readthedocs.io/en/latest/installation.html).([bci.plus][4])

2. **Install g.NEEDaccess Software**:

   * Obtain the g.NEEDaccess client/server software from g.tec. If not provided, contact g.tec support to request access.
   * Install the software on your system following g.tec's installation guidelines.

3. **Set Up LSL Streamer for g.USBamp**:

   * Download the LSL App for g.USBamp from the [Lab Streaming Layer GitHub repository](https://github.com/labstreaminglayer/App-g.Tec/releases).
   * Install and configure the LSL streamer to interface with the g.USBamp device.([github.com][3], [youtube.com][1])

4. **Configure MindAffect BCI**:

   * Use the provided `noisetag_bci2.json` configuration file as a template.
   * Adjust the configuration parameters as needed to match your setup.

5. **Run the System**:

   * Start the g.NEEDaccess server to initialize the g.USBamp device.
   * Launch the LSL streamer to begin streaming EEG data.
   * Run the MindAffect BCI software with the configured settings.([youtube.com][1])

For a visual walkthrough of the setup process, refer to the following video tutorial:

[![Setup Tutorial](https://img.youtube.com/vi/DDpjOlciFrw/0.jpg)](https://www.youtube.com/watch?v=DDpjOlciFrw)

## Contact

For further assistance or inquiries, please contact:

* **Vladislav Mun**: [vladislav.mun@nu.edu.kz](mailto:vladislav.mun@nu.edu.kz)
* **Alternate Email**: [vlad.mun1999@gmail.com](mailto:vlad.mun1999@gmail.com)

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgments

This guide was developed by [Berdakh Abibullaev](https://github.com/berdakh) to facilitate the integration of g.USBamp with the MindAffect BCI system using LSL.([youtube.com][1])

---

*For detailed explanations and methodologies, refer to the documentation and scripts included in the repository.*

If you need further assistance or have specific questions about any script or functionality, feel free to ask!

[1]: https://www.youtube.com/watch?v=DDpjOlciFrw&utm_source=chatgpt.com "Seting up the g.USBAMP (g.tec) with the MindAffect Open Source BCI."
[2]: https://github.com/NeuroTechX/bci-workshop/blob/master/INSTRUCTIONS.md?utm_source=chatgpt.com "bci-workshop/INSTRUCTIONS.md at master - GitHub"
[3]: https://github.com/brain-products/LSL-BrainAmpSeries?utm_source=chatgpt.com "brain-products/LSL-BrainAmpSeries: LSL connector for BrainAmps"
[4]: https://bci.plus/mindaffect-speller-brainproducts/?utm_source=chatgpt.com "Using the MindAffect Speller with Brain Products Amplifiers - BCI plus"
