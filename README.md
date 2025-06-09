<table>
    <tr>
        <td>
            <img src="https://th.bing.com/th/id/OIP.XrokM5iZL6GfjzMfXaJFIQHaHa?rs=1&pid=ImgDetMain" alt="Ari Joseph Khaytser Profile Photo" width="100" style="border-radius:50%;">
        </td>
        <td>
            <h1 style="margin-left: 20px;">Ari Joseph Khaytser</h1>
        </td>
    </tr>
</table>

I am a software developer in the New York City Area. I graduated in 2024 with a Bachelor's and Master's in Computer Science from NYU, with a concentration on artificial intelligence. On this GitHub page, you will find some of my projects outside of work. 

[My LinkedIn](https://www.linkedin.com/in/ari-josephk/)

---

## Sparse Parallel PyTorch on Multicore

This project explores optimizing neural network linear layers by pruning weight matrices and implementing fast, parallel sparse matrix multiplication using custom C++ extensions for PyTorch. The approach leverages both CSR and COO sparse formats and OpenMP for multicore acceleration, aiming to reduce memory usage and improve inference speed with minimal accuracy loss.

**Presentation Video:**

<video width="480" controls>
  <source src="Sparse Parallel PyTorch on Multicore/Multicore Presentation.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Results:**  
The optimized sparse parallel implementation achieved up to 6x speedup on multicore CPUs with over 90% sparsity, while maintaining comparable accuracy to dense baselines.

**Key Features:**
- Pruning of neural network weights for high sparsity
- Custom C++/PyTorch extensions for efficient sparse matrix operations
- Support for CSR and COO formats
- Multithreaded execution with OpenMP for speedup on multicore CPUs

**Documentation & Report:**
- [Final Project Report (PDF)](Sparse%20Parallel%20PyTorch%20on%20Multicore/Multicore_Final_Project_Report.pdf)

**Main Files:**
- [models.py](Sparse%20Parallel%20PyTorch%20on%20Multicore/models.py): Model definitions and PyTorch/C++ integration
- [mlp_lib.cpp](Sparse%20Parallel%20PyTorch%20on%20Multicore/mlp_lib.cpp): C++ extension source code
- [test.py](Sparse%20Parallel%20PyTorch%20on%20Multicore/test.py): Benchmarking and testing script
- [setup.py](Sparse%20Parallel%20PyTorch%20on%20Multicore/setup.py): Build script for the C++ extension
- [readme.md](Sparse%20Parallel%20PyTorch%20on%20Multicore/readme.md): Project-specific setup and usage instructions


For setup and usage, see the [project README](Sparse%20Parallel%20PyTorch%20on%20Multicore/readme.md).


## [Shed Tracker](https://github.com/ari-josephk/Shed-Tracker)
A web tool for tracking the progress of New York City's "Get Sheds Down" initiative, which aims to reduce the number of sidewalk construction sheds. The app fetches daily data from the NYC Department of Buildings, visualizes trends in shed permits, and provides borough-level statistics and reductions over time. Built with Node.js, Express, Python, and JavaScript (Chart.js), it features automated data compilation and a public dashboard.
- [Live Website](https://ari-josephk.github.io/Shed-Tracker/)
- [Source Code](https://github.com/ari-josephk/Shed-Tracker)

## [MidWays](https://github.com/ari-josephk/Midways)
A collaborative web application that helps groups find fair meeting points (e.g., restaurants, parks) equidistant from all members, considering different travel modes. Users can enter multiple starting locations, apply filters, and share maps via unique links. Features include account creation, saving favorite locations/groups, and real-time collaboration. Built with React, Node.js, Express, MongoDB, and Google Maps API.

Utilizes a iterative time-based centroid algorithm that I made with some simple linear argebra. It keeps updating the center point until iterations stop moving it (meaning we reached optimal point), or until we hit a max number of iterations. 


- [Live Demo](https://midways-cloud-run-4tzuhyxh3a-uc.a.run.app/)
- [Source Code](https://github.com/ari-josephk/Midways)


