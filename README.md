# AutomatedGOLE NSI Discovery Documents

Fixed location for those AutomatedGOLE sites that still do not support dynamic discovery.

Documents within this repository are "discovered" by DDS Server instances using a static URL.  For example, a DDS server would be provisioned with the following entry:

	<peerURL type="application/vnd.ogf.nsi.nsa.v1+xml">https://raw.githubusercontent.com/AutomatedGOLE/nsi-discovery-documents/nsa/sinet.ac.jp_2013_nsa.xml</peerURL>

Inside the _NSA Description Document_ you would have an interface element referencing the topology document within the repository:

    <interface>
        <type>application/vnd.ogf.nsi.topology.v2+xml</type>
        <href>https://raw.githubusercontent.com/AutomatedGOLE/nsi-discovery-documents/topology/sinet.ac.jp_2013_nml.xml</href>
    </interface>

Eventually, use of this repository should be discontinued as each NSA either supports direct document discovery or integrated directly with the DDS infrestructure.

