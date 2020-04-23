pyronear.datasets
=================

All datasets are subclasses of :class:`torchvision.datasets.vision.VisionDataset`
i.e, they have ``__getitem__`` and ``__len__`` methods implemented.
Hence, they can all be passed to a :class:`torch.utils.data.DataLoader`
which can load multiple samples parallelly using ``torch.multiprocessing`` workers.

The following datasets are available:

.. contents:: Datasets
    :local:

.. currentmodule:: pyronear.datasets


OpenFire
~~~~~~~~
An image classification dataset for wildfire in natural environments, built using Google Images referenced data.

.. autoclass:: OpenFire

WildFire
~~~~~~~~
A video dataset labeled with spatio-temporal keypoints for wilfire detection, built using available surveillance camera data.

.. autoclass:: WildFireDataset
