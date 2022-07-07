<!--
    Copyright (c) 2022 Robert Bosch Manufacturing Solutions GmbH
    Copyright (c) 2021-2022 Contributors to the Eclipse Foundation

    See the NOTICE file(s) distributed with this work for additional 
    information regarding copyright ownership.
    
    This program and the accompanying materials are made available under the
    terms of the Apache License, Version 2.0 which is available at
    https://www.apache.org/licenses/LICENSE-2.0.
     
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
    License for the specific language governing permissions and limitations
    under the License.
    
    SPDX-License-Identifier: Apache-2.0
-->

# Tractus-X Website
This is the repository for the code of the Tractus-X website hosted at https://eclipse.org/tractusx

## Build Website
The Tractus-X website is using the static website generator framework [Hugo](https://gohugo.io).
Its styling is based on the [hugo-fresh](https://github.com/StefMa/hugo-fresh) theme.
The theme is included as git submodule. So you need to clone the repository by
``
git clone --recurse-submodules https://github.com/eclipse-tractusx/website.git
``
which will also clone the repository of the theme into the themes folder.

To run the page locally just run
``
hugo server
``
from the root of the repository.
