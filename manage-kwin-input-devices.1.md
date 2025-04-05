# manage-kwin-input-devices(1) manpage

## NAME

manage-kwin-input-devices - Manage disable/enable state of input devices under Kwin(works under KDE Wayland)

## DESCRIPTION

This utility lets you to disable input devices under KDE in wayland, for instances like you want to place a mechanical keyboard on your laptop one without worrying hitting any of its keys by accident.

## SYNOPSIS

This is the basic format of the command:

```bash
manage-kwin-input-devices _operation_mode_ _operation_args_...
```

## OPERATION MODES

This section documents the supported commands and their arguments of this command:

### list

```bash
manage-kwin-input-devices list
```

This operation mode lists existing input devices, their sysfs names, and their enabled statuses.

The display name column is formatted in a way that can be directly used as arguments of the enable/disable/toggle operation modes.

### enable

```bash
manage-kwin-input-devices enable _device_...
```

This operation mode enables user-specified input devices.

You can either use the input devices' sysfs names or display names.

### disable

```bash
manage-kwin-input-devices disable _device_...
```

This operation mode disables user-specified input devices.

You can either use the input devices' sysfs names or display names.

### toggle

```bash
manage-kwin-input-devices toggle _device_...
```

This operation mode enables user-specified disabled input devices, and vice-versa.

You can either use the input devices' sysfs names or display names.

### enable-from-file

```bash
manage-kwin-input-devices enable-from-file [_device_list_file_|"_builtin_"]
```

This operation mode enables user-specified input devices specified by a user-specified device list file.

Replace the `_device_list_file_` placeholder text to the actual path of the file with the list of devices to be managed, or specify `_builtin_` (literally), to use a built-in list with common values.

### disable-from-file

```bash
manage-kwin-input-devices disable-from-file [_device_list_file_|"_builtin_"]
```

This operation mode disables user-specified input devices specified by a user-specified device list file.

Replace the `_device_list_file_` placeholder text to the actual path of the file with the list of devices to be managed, or specify `_builtin_` (literally), to use a built-in list with common values.

### toggle-from-file

```bash
manage-kwin-input-devices toggle-from-file [_device_list_file_|"_builtin_"]
```

This operation mode toggles the enabled status of input devices specified by a user-specified device list file.

Replace the `_device_list_file_` placeholder text to the actual path of the file with the list of devices to be managed, or specify `_builtin_` (literally), to use a built-in list with common values.

## EXIT STATUSES

### 0

Operation is successful.

### 1

Program prerequisites not met.

### 2

Generic error occurred.

## ENVIRONMENT

This section documents the supported environment variables that can change this utility's behaviors:

### QDBUS

The `qdbus`-like command to use.

## AUTHORS

This project is based on [Amine Hassane](https://gist.github.com/Sporif)'s work: [Enable or disable input devices on KDE](https://gist.github.com/Sporif/0e52e4b0eaf071cfbf19f3381ba3d65a), it is then enhanced by 林博仁(Buo-ren Lin) for more features.
