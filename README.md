# BROWSER-COIN-HASH
Skip to content
GitLab
Projects
MoreToggle navigation
F
flake8
Project overview
Repository
Files
Commits
Branches
Tags
Contributors
Graph
Compare
Locked Files
Issues
41
Merge Requests
8
Requirements
CI / CD
Security & Compliance
Operations
Analytics
Snippets
Members

Close sidebar
Open sidebar
PyCQA
flake8
Repository
39ceae7491f4121902a5dccc22657a0675c95539
flake8
 example-plugin
 setup.py
 setup.py  1.04 KB
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
# -*- coding: utf-8 -*-
import setuptools
setuptools.setup(
    name='flake8-example-plugin',
    license='MIT',
    version='1.0.0',
    description='Example plugin to Flake8',
    author='Ian Cordasco',
    author_email='graffatcolmingov@gmail.com',
    url='https://gitlab.com/pycqa/flake8',
    package_dir={'': 'src/'},
    packages=['flake8_example_plugin'],
    entry_points={
        'flake8.extension': [
            'X1 = flake8_example_plugin:ExampleOne',
            'X2 = flake8_example_plugin:ExampleTwo',
        ],
    },
    classifiers=[
        'Framework :: Flake8',
        'License :: OSI Approved :: MIT License',
        'Programming Language :: Python',
        'Programming Language :: Python :: 2',
        'Programming Language :: Python :: 2.7',
        'Programming Language :: Python :: 3',
        'Programming Language :: Python :: 3.4',
        'Programming Language :: Python :: 3.5',
        'Topic :: Software Development :: Libraries :: Python Modules',
        'Topic :: Software Development :: Quality Assurance',
    ],
)
